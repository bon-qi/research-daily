# Paper-daily
<!-- ## Aim : recording footprint and introducing new ideas.
1. `Project`: paper rich in pipeline or combine somethig previously.
2. `Paper`: Methodology worth thinking twice.
3. `playground`: Packages / Libraries worth learning from. -->
<!-- Claim: Will read a paper carefully in 1~3 days. -->
> Be the friend of time
<!-- > The people who believe in miracle are those as great as miracle. -->
---
[TOC]

---
### 12.26 2022
**Projects** :
<!-- - (2112.09127, avatar) [ICON](https://github.com/YuliangXiu/ICON): Tutorialiable project for playing around with neural avatars. -->

- (2211.13226, edit nerf) [ClimateNeRF](https://climatenerf.github.io/): 
1. **pipeline**: [pre-trained NGP model] --> traditional physics based rendering + style-transfer --> [snow, flood, smog simulated sence].


**playground**:
- [manim](https://docs.manim.community/en/stable/guides/): fancy animated math formulas with $\LaTeX$ for python.

scene.py: `manim -pql scene.py CreateCircle`
```python 
from manim import *
class CreateCircle(Scene):
    def construct(self):
        circle = Circle()
        circle.set_fill(PINK, opacity=0.5)
        self.play(Create(circle))
```
- [rich](https://rich.readthedocs.io/en/stable/introduction.html): rich text output.  `%load_ext ric` for `Ipython`
```python
from rich.panel import Panel
Panel.fit("[bold yellow]Hi, I'm a Panel", border_style="red")
```
<!-- -  See your fancy `python` terminal output with [rich](https://github.com/Textualize/rich)!
- My pleasure to help the community for translation in docs one day... -->
---
### 12.27 2022
- (2212.05231, NGP+NeuS)[NeuS2](https://vcai.mpi-inf.mpg.de/projects/NeuS2/):
1. **pipeline**:  [NeRF input] --> NeuS + InstantNGP, add second derivation for efficient optimization, method for dynamic scene (loss consistency) --> [NeuS model].
2. **inspiration**: InstantNGP can help a lot for development, can also integrate with some small utils (dynamic scene).

---
### 12.28 2022
- (2212.10699, basis of nerf)[PlatteNeRF](https://arxiv.org/pdf/2212.10699.pdf): 
1. **Abstract**: decomposing a NeRF into color basis for editting.
2. **Code**: 
2. **Inspiration**: segmentation/recongnition of NeRF models.

---
### 12.29 2022
- (2211.05783, SfM, flow)[UniMatch](https://arxiv.org/abs/2211.05783): 
1. **Idea**: A unified framework for optical flow, stereo match and depth estimation with transformers.
2. **Pipeline**: transformer, accross-attention.
<!-- 3. **Inspiration** -->

**playground**
* Try out and explore [transformers](https://huggingface.co/docs/transformers/index) and [diffusion model](https://huggingface.co/docs/diffusers/quicktour) with hugging-face!

---
Driver's license, new year holiday.

--- 
### 1.4 2023

- **(2112.07945, head NeRF)[EG3D](https://github.com/NVlabs/eg3d)**: 
1. **Implementation**: remarkable [dnnlib.utils.construct_class_by_name](https://github.com/NVlabs/eg3d/blob/main/eg3d/dnnlib/util.py), `module = importlib.module('[MODULE_PATH]')` and `obj = attr(module,"[ATTR_NAME]")`. [click](https://click.palletsprojects.com/en/8.1.x/) for better `argparse` to a function.[eg3d.eg3d.viz](https://github.com/NVlabs/eg3d/tree/main/eg3d/viz) for `imgui` based interface with 3d-data, refer [eg3d.eg3d.visualizer.Visualizer](https://github.com/NVlabs/eg3d/blob/main/eg3d/visualizer.py) for how to rewrite. 
2. **Idea**: `triplane`: a balance between `octree` and `positonal emebdding`, standard improving of images: super-resolution, pyramid to discrimator. [TO BE CAREFULLY]: supplemental details.
3. Datasets: `FFHQ` for human head, `` for cat head.

**playground**: a survey of **torch.Tensor.device**
- A suvey of `torch.Tensor.device` between: `cpu, cuda, ipu, xpu, mkldnn, opengl, opencl, ideep, hip, ve, fpga, ort, xla, lazy, vulkan, mps, meta, hpu`
- `opengl, vulkan` need compile from source, aim at  mobile device deployment.
- `mps` for apple cheaps,  `meta` for [a fake tensor](https://huggingface.co/blog/accelerate-large-models)(all platforms).
- Benchmark: speed, difference in using.

--- 
### 1.6 2023
- (2011.13961, dynamic NeRF)[D-NeRF](https://github.com/albertpumarola/D-NeRF): 
1. Implementation: Based on [NeRF-PyTorch](https://github.com/yenchenlin/nerf-pytorch).
2. Paper: [dynamic images] -> [canonical space, time disturb, NeRF model] -> [D-NeRF]

### 1.8 2023
**playground**
- [PyWebview](https://pywebview.flowrl.com/guide/) for a web-based GUI (w/ `html`) for python. (Further: `Flask`) , other solutions: [PySimpleGUI](https://www.pysimplegui.org/en/latest/)(super easy to use), [PyImGui](https://pyimgui.readthedocs.io/en/latest/guide/first-steps.html)(graphics usage).

---
### 1.9 2023
- (1703.10593, 1611.07004)[CycleGAN and Pix2Pix](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix): 
1. **Pipeline** (CycleGAN): $Id = G_X G_Y$ as prior to supervision,$Loss_{G_X, G_Y} + \lambda Loss_{Id}$, paired data avoided.
2. Project: borrowed implementation (for $G, D$), super nice and standard [NEED FURTHER READ].

- (1912.04958)[StyleGAN](https://github.com/lucidrains/stylegan2-pytorch): YOLO in image-gans.
1. **Pipeline**: 
2. **Inspiration**: 

### 1.10 2023
* **Playground**: making a bot of `wechat` or `QQ` to automatically send and reply.s

### 1.11 2023
- [torch-ngp](): fast, pipelinable project, [ngp-pl]() for another.
- Javascript + Node.js for web backend.

### 1.14 2023
**playground**
- [wandb](https://wandb.ai) : for logging trainning things (better).

### 1.15 - 1.20 2023
**playground**

- [Unreal Engine 5](https://docs.unrealengine.com/4.27/zh-CN/): aim: avatar, virtual reality.
- [Blender]()
- [Vulkan](https://wiki.archlinux.org/title/Vulkan): for modern ray tracing.
- [electron](https://www.electronjs.org/zh/docs/latest/s): node.js + html + chrome ==> app!
- [streamlit](https://streamlit.io) : a quick gui maker based on web. 

- [Arch Linux](https://wiki.archlinux.org/): pacman+aur (fruitful), simplicity. i3wm + neovim + i3status-rs! (xorg)
- [lazygit]()
- [neovim]()
- [i3wm](): dmenu
- []

### 1.20 - 1.24 2023
Keywords: "Spring Festival", "Websipder"
**playground**

- [selenium]() : automatically using web-browser
- [yt-dlp]() : a downloader for youtube.com, bilibili.com, etc.. 

### 1.20 - 1.31 2023
Keywords: contralable NeRF

- (2301.10241, representation of 3d geometry)[k-planes](https://arxiv.org/pdf/2301.10241.pdf): a high-level of representation.
- (2112.05139, text-guided NeRF)[CLIPNeRF](https://arxiv.org/pdf/2112.05139.pdf): conditional model, NeRF lantent space.

## Demos
The key idea of this fold is:
1. standard usage of some library.
2. some good code with fine structure/trick in any project.

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
**playground**
* Try out and explore [transformers](https://huggingface.co/docs/transformers/index) and [diffusion model](https://huggingface.co/docs/diffusers/quicktour) with hugging-face!

**playground**: a survey of **torch.Tensor.device**
- A suvey of `torch.Tensor.device` between: `cpu, cuda, ipu, xpu, mkldnn, opengl, opencl, ideep, hip, ve, fpga, ort, xla, lazy, vulkan, mps, meta, hpu`
- `opengl, vulkan` need compile from source, aim at  mobile device deployment.
- `mps` for apple cheaps,  `meta` for [a fake tensor](https://huggingface.co/blog/accelerate-large-models)(all platforms).
- Benchmark: speed, difference in using.

### 1.8 2023
**playground**
- [PyWebview](https://pywebview.flowrl.com/guide/) for a web-based GUI (w/ `html`) for python. (Further: `Flask`) , other solutions: [PySimpleGUI](https://www.pysimplegui.org/en/latest/)(super easy to use), [PyImGui](https://pyimgui.readthedocs.io/en/latest/guide/first-steps.html)(graphics usage).

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



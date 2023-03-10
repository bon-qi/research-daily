# Paper-Weekly

> Be the friend of time.

---
[TOC]

---
## 12/26/2022 ~ 14/2/2023 (refined during 7/3/2023 ~)

---
- (2112.09127, avatar) [ICON](https://github.com/YuliangXiu/ICON): Tutorialiable project for playing around with neural avatars.
- (2211.13226, editable nerf) [ClimateNeRF](https://climatenerf.github.io/): 
1. **pipeline**: [pre-trained NGP model] --> traditional physics based rendering + style-transfer --> [snow, flood, smog simulated sence].

---
- (2212.05231, NGP+NeuS)[NeuS2](https://vcai.mpi-inf.mpg.de/projects/NeuS2/):
1. **pipeline**:  [NeRF input] --> NeuS + InstantNGP, add second derivation for efficient optimization, method for dynamic scene (loss consistency) --> [NeuS model].
2. **inspiration**: InstantNGP can help a lot for development, can also integrate with some small utils (dynamic scene).

---
- (2212.10699, basis of nerf)[PlatteNeRF](https://arxiv.org/pdf/2212.10699.pdf): 
1. **Abstract**: decomposing a NeRF into color basis for editting.
2. **Code**: 
2. **Inspiration**: segmentation/recongnition of NeRF models.

---
- (2211.05783, SfM, flow)[UniMatch](https://arxiv.org/abs/2211.05783): 
1. **tl;dr**: A unified framework for optical flow, stereo match and depth estimation with transformers.
2. **Pipeline**: transformer, accross-attention.

---
Driver's license, new year holiday.

--- 
- **(2112.07945, head NeRF)[EG3D](https://github.com/NVlabs/eg3d)**: 
1. **Implementation**: remarkable [dnnlib.utils.construct_class_by_name](https://github.com/NVlabs/eg3d/blob/main/eg3d/dnnlib/util.py), `module = importlib.module('[MODULE_PATH]')` and `obj = attr(module,"[ATTR_NAME]")`. [click](https://click.palletsprojects.com/en/8.1.x/) for better `argparse` to a function.[eg3d.eg3d.viz](https://github.com/NVlabs/eg3d/tree/main/eg3d/viz) for `imgui` based interface with 3d-data, refer [eg3d.eg3d.visualizer.Visualizer](https://github.com/NVlabs/eg3d/blob/main/eg3d/visualizer.py) for how to rewrite. 
2. **Idea**: `triplane`: a balance between `octree` and `positonal emebdding`, standard improving of images: super-resolution, pyramid to discrimator. [TO BE CAREFULLY]: supplemental details.
3. Datasets: `FFHQ` for human head, `` for cat head.

--- 
- (2011.13961, dynamic NeRF)[D-NeRF](https://github.com/albertpumarola/D-NeRF): 
1. Implementation: Based on [NeRF-PyTorch](https://github.com/yenchenlin/nerf-pytorch).
2. Paper: [dynamic images] -> [canonical space, time disturb, NeRF model] -> [D-NeRF]

---
- (1703.10593, 1611.07004)[CycleGAN and Pix2Pix](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix): 
1. **Pipeline** (CycleGAN): $Id = G_X G_Y$ as prior to supervision,$Loss_{G_X, G_Y} + \lambda Loss_{Id}$, paired data avoided.
2. Project: borrowed implementation (for $G, D$), super nice and standard [NEED FURTHER READ].

---
- (1912.04958)[StyleGAN](https://github.com/lucidrains/stylegan2-pytorch): YOLO in image-gans.
1. **Pipeline**: 
2. **Inspiration**: 

---
Keywords: contralable NeRF
- (2301.10241, representation of 3d geometry)[k-planes](https://arxiv.org/pdf/2301.10241.pdf): a high-level of representation.
- (2112.05139, text-guided NeRF)[CLIPNeRF](https://arxiv.org/pdf/2112.05139.pdf): conditional model, NeRF lantent space.

---

TODO:
> Transformer (attention is all you need)


---


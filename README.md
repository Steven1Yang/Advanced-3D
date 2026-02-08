# Advanced-3D
An overview of 3d vision

# Reconstruction
- **PanSplat**  
  📄 https://arxiv.org/abs/2412.12096  
  💻 https://github.com/chengzhag/PanSplat  
 _Tags_: `3DGS`, `panorama`, `feed-forward`,`feature pyramid network`  
TLDR：A feed-forward method to reconstruct gaussians scene, enable the use of high resolution panorama images as input.

- **OmniGS**  
  📄 https://arxiv.org/abs/2404.03202  
  💻 https://github.com/liquorleaf/OmniGS  
 _Tags_: `3DGS`, `panorama`, `optimization`,`rasterization`  
TLDR：A 3DGS reconstruction method based on optimization was proposed, and a rasterization renderer for panoramic images was designed.

- **SC-OmniGS**  
  📄 https://arxiv.org/abs/2502.04734  
  💻 https://github.com/chenyingshu/sc-omnigs  
 _Tags_: `3DGS`, `panorama`, `optimization`,`self-calibrating`   
TLDR：An optimization-based 3D Gaussian Splatting reconstruction method for panoramic images, which is able to self-calibrate camera poses using only image inputs, and rectifies the panoramic sphere to reduce distortion effects.

# Generation 
- **DiT**  
  📄 https://arxiv.org/abs/2212.09748  
  💻 https://github.com/facebookresearch/DiT  
 _Tags_: `diffusion`, `transformer`, `feed-forward`    
TLDR：A feed-forward Transformer-based latent diffusion model that replaces U-Nets and exhibits strong compute–quality scaling.

# Depth Estimation
- **Depth Any Panoramas**  
  📄 https://arxiv.org/abs/2512.16913  
  💻 https://github.com/Insta360-Research-Team/DAP   
 _Tags_: `depth`, `panorama`, `feed-forward`,`pseudo-label`  
TLDR：A feed-forward method to get the depth map of panoramas, using the pseudo label to guarantee the quality of datasets.

# Mathematical Fundamentals
- **Spherical Position Encoding**  
  📄 https://arxiv.org/abs/2310.04454  
 _Tags_: `position encoding`, `spherical`, `RoPE`   
TLDR：A RoPE-based spherical position encoding method that can function in a spherical coordinate system.

- **SpRePE**  
  📄 coming soon  
  💻 https://anonymous.4open.science/r/SpRePE-7357/README.md  
 _Tags_: `position encoding`, `spherical`, `RoPE`, `ViT`   
TLDR：A new paradigm of position encoding for spherical scene, not the RoPE-based one.

## NeRF & Radiance Fields
- **Mip-NeRF 360**  
  https://arxiv.org/abs/2111.12077  
  _Tags_: `360`, `anti-aliasing`, `ray-aware`


# 3D Gaussian Splatting

## Core
- **3D Gaussian Splatting** (SIGGRAPH 2023)  
  📄 https://arxiv.org/abs/2308.04079  
  💻 https://github.com/graphdeco-inria/gaussian-splatting  

## Semantic / Editing
- **Gaussian Grouping** (CVPR 2024)  
  📄 https://arxiv.org/abs/2403.XXXXX  
  💻 https://github.com/lkeab/gaussian-grouping  

# Feed-forward 3D Reconstruction
- **CUT 3R**
  📄
  💻

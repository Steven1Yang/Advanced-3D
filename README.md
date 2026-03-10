# Advanced-3D
An overview of 3d vision

# Reconstruction
- **PanSplat**  
  📄 https://arxiv.org/abs/2412.12096  
  💻 https://github.com/chengzhag/PanSplat  
 _Tags_: `3DGS`, `panorama`, `feed-forward`,`feature pyramid network`  
TLDR:A feed-forward method to reconstruct gaussians scene, enable the use of high resolution panorama images as input.

- **OmniGS**  
  📄 https://arxiv.org/abs/2404.03202  
  💻 https://github.com/liquorleaf/OmniGS  
 _Tags_: `3DGS`, `panorama`, `optimization`,`rasterization`  
TLDR:A 3DGS reconstruction method based on optimization was proposed, and a rasterization renderer for panoramic images was designed.

- **SC-OmniGS**  
  📄 https://arxiv.org/abs/2502.04734  
  💻 https://github.com/chenyingshu/sc-omnigs  
 _Tags_: `3DGS`, `panorama`, `optimization`,`self-calibrating`   
TLDR:An optimization-based 3D Gaussian Splatting reconstruction method for panoramic images, which is able to self-calibrate camera poses using only image inputs, and rectifies the panoramic sphere to reduce distortion effects.

# Generation 
- **DiT**  
  📄 https://arxiv.org/abs/2212.09748  
  💻 https://github.com/facebookresearch/DiT  
 _Tags_: `latent diffusion`, `transformer`, `feed-forward`    
TLDR:A feed-forward Transformer-based latent diffusion model that replaces U-Nets and exhibits strong compute–quality scaling.

- **WorldStereo**  
  📄 https://arxiv.org/abs/2603.02049  
  💻 https://github.com/FuchengSu/WorldStereo
 _Tags_: `controlnet`, `multi-bi`, `long sequence`    
TLDR:A novel camera-guided video generation framework tailored for 3D reconstruction, introducing two dedicated geometric memory modules to enable precise camera control and multi-view consistent content generation, facilitating high-quality 3D scene reconstruction while supporting efficient inference via a distilled VDM backbone without joint fine-tuning.

- **VBench**  
  📄 https://arxiv.org/abs/2311.17982  
  💻 https://github.com/Vchitect/VBench  
 _Tags_: `benchmark`, `multidimensional-evaluation`, `prompt-suite`, `human alignment`    
TLDR:A comprehensive benchmark for evaluating video generation models (e.g., text-to-video), introducing 16 fine-grained evaluation dimensions, carefully designed prompt suites, and large-scale human preference annotations to ensure strong alignment with human perception, enabling deeper analysis and improvement of video generation systems.

# Depth Estimation
- **Depth Any Panoramas**  
  📄 https://arxiv.org/abs/2512.16913  
  💻 https://github.com/Insta360-Research-Team/DAP   
 _Tags_: `depth`, `panorama`, `feed-forward`,`pseudo-label`  
TLDR:A feed-forward method to get the depth map of panoramas, using the pseudo label to guarantee the quality of datasets.

# Mathematical Fundamentals
- **Spherical Position Encoding**  
  📄 https://arxiv.org/abs/2310.04454  
 _Tags_: `position encoding`, `spherical`, `RoPE`   
TLDR:A RoPE-based spherical position encoding method that can function in a spherical coordinate system.

- **SpRePE**  
  📄 coming soon  
  💻 https://anonymous.4open.science/r/SpRePE-7357/README.md  
 _Tags_: `position encoding`, `spherical`, `RoPE`, `ViT`   
TLDR:A new paradigm of position encoding for spherical scene, not the RoPE-based one.

- **RayRoPE**  
  📄 https://arxiv.org/abs/2601.15275  
  💻 https://github.com/Lucas-707/RayRoPE  
  _Tags_: `position encoding`, `cross-views`, `RoPE`, `Raymap`  
TLDR:A new method to encode cross views input, which can maintain the consistency of the geometry struction.  

# Benchmark

- **VBench**  
  📄 https://arxiv.org/abs/2311.17982  
  💻 https://github.com/Vchitect/VBench  
 _Tags_: `video generation`, `benchmark`     
TLDR:A novel benchmark for video generation,which contains more dimensions than former methods.

- **WorldScore**  
  📄 https://arxiv.org/abs/2504.00983  
  💻 https://github.com/haoyi-duan/WorldScore?tab=readme-ov-file  
 _Tags_: `video generation`, `benchmark`, `dynamic`     
TLDR:A benchmark for video generation, which is more comprehensive than VBench, using dynamic and static metrics to measuring the quality of generated videos and generating model.

## Semantic / Editing
- **Gaussian Grouping** (CVPR 2024)  
  📄 https://arxiv.org/abs/2403.XXXXX  
  💻 https://github.com/lkeab/gaussian-grouping  

# Feed-forward 3D Reconstruction
- **CUT 3R**
  📄
  💻

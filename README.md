# Advanced_papers_reading
An overview of read papers in recent.

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

- **Wan**  
  📄 https://arxiv.org/abs/2503.20314  
  💻 https://github.com/Wan-Video/Wan2.2?tab=readme-ov-file  
 _Tags_: `diffusion transformer`, `scalable pre-training`, `multi-task video generation`    
TLDR:a comprehensive and open suite of video foundation models built on the diffusion Transformer paradigm, designed to advance video generation capabilities. Leveraging innovations such as a novel VAE, scalable pre-training strategies, large-scale data curation, and automated evaluation metrics, Wan achieves state-of-the-art performance in video quality, temporal consistency, and multi-task adaptability. The suite includes both 1.3B and 14B parameter models, supporting a wide range of tasks, including image-to-video generation, instruction-guided video editing, and personalized video synthesis. Wan is fully open-sourced, enabling both academic research and industrial applications while remaining resource-efficient and compatible with consumer-grade GPUs.

- **Context-as-Memory**  
  📄 https://arxiv.org/abs/2506.03141
  💻 coming soon
_Tags_: `diffusion transformer`, `memory bank`, `video to video`, `long sequence videos`
TLDR:a video to video method to predict video frames, uses historical video frames as context to enhance the result of generation，which can generate hight consistent long sequence video.

- **InSpatiol-WorldFM**  
  📄 https://arxiv.org/abs/2603.11911  
  💻 https://github.com/inspatio/worldfm  
 _Tags_: `diffusion transformer`, `frame model`, `3D construction condition`    
TLDR:a light method to generate videos with frame model，maintaining consistency between different frames，which uses model distillation to reduce the steps of diffusion to achieve real-time rendering.This method only use the self-attention to predict the target latent, and it has been proved to gain better result than cross-attention one's.

- **InSpatiol-World**  
  📄 coming soon  
  💻 https://github.com/inspatio/inspatio-world?tab=readme-ov-file  
 _Tags_: `diffusion transformer`, `frame model`, `3D construction condition`, `text condition`    
TLDR:

- **WorldStereo**  
  📄 https://arxiv.org/abs/2603.02049  
  💻 https://github.com/FuchengSu/WorldStereo   
 _Tags_: `controlnet`, `multi-bi`, `long sequence`    
TLDR:A novel camera-guided video generation framework tailored for 3D reconstruction, introducing two dedicated geometric memory modules to enable precise camera control and multi-view consistent content generation, facilitating high-quality 3D scene reconstruction while supporting efficient inference via a distilled VDM backbone without joint fine-tuning.

- **Stereo World Model**  
  📄 https://arxiv.org/abs/2603.17375  
  💻 https://github.com/SunYangtian/StereoWorld   
 _Tags_: `new attn method`, `stereo videl`, `camera position encoding`    
TLDR:A method to generate stereo video, this method proposes a new attention method using single attention in one view and using the cross attention of different viewsinstead of concatnating two tokens from different cameras to decrease the consume of GPUs, this method also proposes a camera position encoding method to connect two views.

- **Context-forcing**  
  📄 https://arxiv.org/abs/2602.06028  
  💻 https://github.com/TIGER-AI-Lab/Context-Forcing     
 _Tags_: `self-forcing`, `distill`, `real-time`    
TLDR:A method to generate long-sequence video,which contains more than one minutes long frames,with casual structure and self-forcing method.

# 4D generation
- **BulletTime**  
  📄 https://arxiv.org/abs/2512.05076  
  💻 https://19reborn.github.io/Bullet4D/  
 _Tags_: `dynamic`, `time-control`, `decoupling`  
TLDR:BulletTime injects world time and camera pose as two independent controls into a video diffusion model to decouple scene dynamics from camera motion, but it still lacks an explicit static-dynamic 4D scene representation.

- **4Real-Video**  
  📄 https://arxiv.org/pdf/2412.04462  
  💻 https://snap-research.github.io/4Real-Video/  
 _Tags_: `time consist`, `space consist`, `decoupling`  
TLDR:4Real Video generates a spatio temporally consistent 4D video grid from a fixed view video and a freeze time video by synchronizing temporal and viewpoint streams inside a diffusion transformer.

- **DreamDrive**  
  📄 https://arxiv.org/abs/2501.00601  
  💻 https://jiageng.me/DreamDrive/  
 _Tags_: `diffusion`, `dynamic-static decoupling`,   
TLDR:DreamDrive is a generative 4D driving scene modeling framework from street view images. It first uses a driving video diffusion prior to synthesize 2D reference images, then lifts them into 3D with multiview stereo and Gaussian initialization. A self supervised decomposition module, based on rendering error maps, dynamic scoring, and spatio temporal clustering, separates static backgrounds from dynamic objects. The final hybrid Gaussian representation uses time independent Gaussians for static structures and time dependent Gaussians for moving objects. Given any ego vehicle trajectory, DreamDrive renders 3D consistent dynamic driving videos via Gaussian Splatting, enabling controllable scene generation, novel view synthesis, and downstream support for perception and planning.

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
 _Tags_: `benchmark`, `multidimensional-evaluation`, `prompt-suite`, `human alignment`    
TLDR:A comprehensive benchmark for evaluating video generation models (e.g., text-to-video), introducing 16 fine-grained evaluation dimensions, carefully designed prompt suites, and large-scale human preference annotations to ensure strong alignment with human perception, enabling deeper analysis and improvement of video generation systems.

- **WorldScore**  
  📄 https://arxiv.org/abs/2504.00983  
  💻 https://github.com/haoyi-duan/WorldScore?tab=readme-ov-file  
 _Tags_: `video generation`, `benchmark`, `dynamic`     
TLDR:A benchmark for video generation, which is more comprehensive than VBench, using dynamic and static metrics to measuring the quality of generated videos and generating model.


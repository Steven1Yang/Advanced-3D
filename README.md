# Advanced_papers_reading
An overview of read papers in recent.

# AR(DMD)
- **One forcing**  
  📄 https://arxiv.org/abs/2605.23458  
  💻 https://github.com/Aurora-edu/One-Forcing  
 _Tags_: `GAN`, `DMD`, `one-step`, `video generation`    
TLDR:To solve the problem of miss-match between generated data and real data of one-step distillation, this method introduced a GAN to distiiation model to discriminate the quality of generated one.

- **DreamFusion(SDS)**  
  📄 https://arxiv.org/abs/2209.14988  
  💻 https://github.com/ashawkey/stable-dreamfusion   
 _Tags_: `SDS`, `distribution match`, `generation`    
TLDR:The score distillation sampling method of this paper is of vital importance to distillation, it uses the frozen diffusion model to train another parameter, in detail, this method first adds noise to the generator as the DDPM does at timesteps T, and then uses the score of teacher model to guide how we should move the zt=atg+.., and since the noise is an uncorrected item, so the corrected item must be the atg, which we can use the chain function to update the parameters of g, and then we can get the desired result. 

# Generation
- **DDPM**  
  📄 https://arxiv.org/abs/2006.11239  
  💻 https://github.com/hojonathanho/diffusion  
 _Tags_: `Diffusion`, `generation`    
TLDR:Classical diffusion model,this one is a random generation model, can not controllable generate. Reading this aim to get the original idea of generation and get the details of diffusion model. 

- **DDIM**  
  📄 https://arxiv.org/abs/2010.02502  
  💻 https://github.com/ermongroup/ddim  
 _Tags_: `Diffusion`, `generation`, `ODEs`    
TLDR:An acceleration method of DDPM, this method changes the depends on the Markov chain of reverse sampling process, to make the sampling process faster, and also generalizes it to the perspective of ODEs.

- **Score SDEs**  
  📄 https://arxiv.org/abs/2011.13456  
  💻 https://github.com/yang-song/score_sde   
 _Tags_: `Diffusion`, `generation`, `SDEs`, `discrete‑to‑continuous`    
TLDR:A method to unify the discrete process of diffusion to a continuous SDE formula, which changes the sampling process from "prediction noise - solve - prediction noise" to "prediction score - solve - prediction score",what's the most important is this method change the sampling formula from fixed one-step one to continuous reverse SDE with optional numerical solver, and also offers a method for conditioned generation. 

- **Flow Matching**  
  📄 https://arxiv.org/abs/2210.02747  
  💻 https://github.com/facebookresearch/flow_matching   
 _Tags_: `Diffusion`, `generation`, `velocity field`      
TLDR:This method makes two innovation in my opinion, the first one is that the training trajectory is changed from the gradient of SDEs of "Score SDEs" to the velocity field by constructing a OT-path which is a staight line between the desired data x1 and gaussian noise data x0, so the desired vbelocity always be a constant function x1-x0,and the second one is that this method changes the sampling way, which uses the velocity to guide the current data xT how to move in the current sampling time T.In sampling stage, this method uses (T,xT) as the input, and the network here predicts the velocity of whole data distribution. 

- **Rectified Flow**  
  📄 https://arxiv.org/abs/2209.03003  
  💻 https://github.com/gnobitab/RectifiedFlow   
 _Tags_: `Diffusion`, `generation`, `velocity field`, `ODEs`      
TLDR:This method is a improvement of Flow matching,the former one tries to directly get the velocity field instead of the gradient, but it ignores the quality of the path, which may produce the cross point influcing the samping process.The Rectified Flow does the refine process to make the path straight to accelerate the sampling process and increase the determinism of sampling.In detail, after the first train of Flow matching, Rectified Flow uses the sampled X0 as Z0 without sampling from gaussian noise again, and it will get a endpoint by soloving the ODE equation via euler method, when gets the endpoint Z1, it will train the velocity network via the new interpolation line Z0,Z1, since the Z0 and Z1 are deterministic parameters, so the line will be more deterministic and efficient.

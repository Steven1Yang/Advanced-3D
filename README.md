# Advanced_papers_reading
An overview of read papers in recent.

# AR(DMD)
- **One forcing**  
  📄 https://arxiv.org/abs/2605.23458  
  💻 https://github.com/Aurora-edu/One-Forcing  
 _Tags_: `GAN`, `DMD`, `one-step`, `video generation`    
TLDR:To solve the problem of miss-match between generated data and real data of one-step distillation, this method introduced a GAN to distiiation model to discriminate the quality of generated one. 

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



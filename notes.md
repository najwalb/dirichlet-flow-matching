# understanding why the samples are all the same 
- could be not enough training
  - in the early steps of diffusion (denoising steps? or also not trained enough denoiser?) samples from the prior would lead to the same denoised point... 
    - the issue is the denoiser logits are too close within a single batch, is this smthg expected in a correct setup?
    - how does diffusion behave (classifier output, vf value, sample output) at each denoising step (early vs late), and why
    - 
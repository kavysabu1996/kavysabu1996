---
layout: post
title:  "Understanding Stable Diffusion: A Comprehensive Guide to the Fundamentals of the Powerful Deep Learning Technique"
date:   2023-02-27 12:27:33 +0530
categories: jekyll update
---
Stable diffusion is an open-source implementation of Latent Diffusion 

**What exactly is the concept of diffusion in deep learning?** \\
The process of progressively adding noise to an image is commonly referred to as 'diffusion' in the context of deep learning. A deep learning model that utilizes the diffusion process to model the probability distribution of a dataset is commonly referred to as a diffusion model. The diffusion process involves adding progressively more noise to the data to smooth it out, and the model is trained to invert this process by generating a sample from the probability distribution represented by the diffusion process.

The two main processes involved are:

1.  forward diffusion : add noise to the image
2.  reverse diffusion : remove noise from the image

Diffusion models require significant computational resources. To deal with this issue "[High-Resolution Image Synthesis with Latent Diffusion Models](https://arxiv.org/pdf/2112.10752.pdf)" introduced latent diffusion models (LDMs). Here, we utilize encoders to reduce the data into a low-dimensional latent space, and then perform the diffusion process on the reduced data. As the resule, both forward and backward diffusions take place in the latent space. Consequently, this approach can significantly reduce the computational cost. 

We can rewrite the primary process in Latent Diffusion Models as follows:
1. forward diffusion : add noise to data in latent space
2. reverse diffusion : remove noise from data in latent space




references :  
[coffee-bean][coffee-bean] \
[https://medium.com/@steinsfu/stable-diffusion-clearly-explained-ed008044e07e][medium1] \
[https://medium.com/@steinsfu/diffusion-model-clearly-explained-cd331bd41166][medium2].

[coffee-bean]: https://www.youtube.com/watch?v=J87hffSMB60
[medium1]:   https://medium.com/@steinsfu/stable-diffusion-clearly-explained-ed008044e07e
[medium2]: https://medium.com/@steinsfu/diffusion-model-clearly-explained-cd331bd41166
# Realism-SD
Exploring various AI models, including community-finetuned checkpoints, custom models, Mixture of models, LoRAs. <br>

I will try to prioritize _photorealism_, _steerability_(the ability to control image details according to possible different complex prompts), and _optimization_ of processing time and resources. <br>

## Models
* [Realistic Vision](https://civitai.com/models/4201/realistic-vision-v60-b1 "Realistic Vision 6.0") :Creating visuals that are virtually identical to reality is the goal of the pioneering Stable Diffusion Model known as Realistic Vision. It accomplishes this by means of a training procedure that is so well thought out that it manages to combine the fictitious with the real, with almost photographic perfection.<br> 
* [Epic Realism](https://civitai.com/models/25694/epicrealism): Epic Realism is an innovative combination of AI and art. It’s a Stable Diffusion Model that elevates creativity to a whole new level, producing realistic visuals that are only fittingly referred to as epic. Its ability to bring digital landscapes to life and dissolve the lines between the real and the imagined makes this approach important in industries like visual storytelling and entertainment.<br>
* [Next Photo](https://civitai.com/models/84335/nextphoto): NextPhoto is the solution for those looking to take photorealistic picture production to the next level. With careful training, this Stable Diffusion Model can produce photos that are so realistic, they might pass for official studio shots.
## Samplers: 
* Euler and Euler Ancestral: Euler is the default scheduler in Invoke. Known for their speed, these schedulers generally require fewer steps to produce high-quality outputs.<br>
* Denoising Diffusion Implicit Models (DDIM): One of the first schedulers used with Stable Diffusion, DDIM is designed for efficiency, offering substantial speed-ups in processing time.<br>
* DPM: These schedulers approximate solutions of differential equations in image quality improvement, with both single-step and multi-step variants available.<br>
* DPM2 Karras and DPM2 Ancestral Karras: DPM2 Karras allows fine control over image generations, while DPM2 Ancestral Karras enhances diversity and explores novel image spaces. DPM2 Karras excel in providing well controlled & diverse generation outputs.<br>

## Upscalling:
* ESRGAN: Before diving into the ESRGAN first let’s get a high-level understanding of the GAN. GANs are capable of generating Fake data that looks realistic. Some of the GAN applications are to enhance the quality of the image. The high-level architecture of the GAN contains two main networks namely the generator network and the discriminator network. The generator network tries to generate the fake data and the discriminator network tries to distinguish between real and fake data, hence helping the generator to generate more realistic data.
ESRGAN is a combination of generative adversarial networks (GANs) and deep convolutional neural networks (CNNs) and it produces highly realistic high-resolution images from low-resolution images.  ESRGAN also has Residual in Residual Dense Block(RRDB) which combines multi-level residual network and dense connection without Batch Normalization.
This model was used to upscale the 512x512 images to desired 2048x2048 size.



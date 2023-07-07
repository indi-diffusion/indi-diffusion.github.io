<div align="center">
<h2>Inversion by Direct Iteration: An Alternative to Denoising Diffusion for Image Restoration</h2>

<h4><a href="https://mdelbra.github.io/">Mauricio Delbracio</a> and <a href="http://milanfar.org">Peyman Milanfar</a></h4>
<h4>Google Research</h4><br>

<a href="https://arxiv.org/abs/2303.11435">[arXiv]</a>
<a href="https://openreview.net/forum?id=VmyFF5lL3F">[openreview]</a>
<a href="https://docs.google.com/presentation/d/1i2h65EFn_pvAe3Jk1a7_bsx4z1enxmPcZtziE2ytOnc/edit?resourcekey=0-6onZxKGPM6obo1uVkH-pQQ#slide=id.g209adefda4f_2_4905">[slides]</a><br><br>

</div>

<p align="justify">
Inversion by Direct Iteration (InDI) is a new formulation for supervised image restoration that avoids the so-called <em>regression to the mean</em> effect and produces more realistic and detailed images than existing regression-based methods. It does this by gradually improving image quality in small steps, similar to generative denoising diffusion models.
</p>

<p align="justify">
Image restoration is an ill-posed problem where multiple high-quality images are plausible reconstructions of a given low-quality input. Therefore, the outcome of a single step regression model is typically  an aggregate of all possible explanations, therefore lacking details and realism. The main advantage of InDI is that it does not try to predict the clean target image in a single step but instead gradually improves the image in small steps, resulting in better perceptual quality.
</p>

<p align="justify">
While generative denoising diffusion models also work in small steps, our formulation is distinct in that it does not require knowledge of any analytic form of the degradation process. Instead, we directly learn an iterative restoration process from low-quality and high-quality paired examples. InDI can be applied to virtually any image degradation, given paired training data. In conditional denoising diffusion image restoration the denoising network generates the restored image by repeatedly denoising an initial image of pure noise, conditioned on the degraded input. Contrary to conditional denoising formulations, InDI directly proceeds by iteratively restoring the input low-quality image, producing high-quality results on a variety of image restoration tasks, including motion and out-of-focus deblurring, super-resolution, compression artifact removal, and denoising.
</p>


### Citation

```
@article{delbracio2023inversion,
title={Inversion by Direct Iteration: An Alternative to Denoising Diffusion for Image Restoration},
author={Mauricio Delbracio and Peyman Milanfar},
journal={Transactions on Machine Learning Research},
issn={2835-8856},
year={2023},
url={https://openreview.net/forum?id=VmyFF5lL3F},
note={Featured Certification}
}
```

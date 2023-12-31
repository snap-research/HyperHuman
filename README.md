# HyperHuman: Hyper-Realistic Human Generation with Latent Structural Diffusion

[Xian Liu](https://alvinliu0.github.io/)<sup>1,2</sup>, [Jian Ren](https://alanspike.github.io/)<sup>1</sup>, [Aliaksandr Siarohin](https://aliaksandrsiarohin.github.io/aliaksandr-siarohin-website/)<sup>1</sup>, [Ivan Skorokhodov](https://universome.github.io/)<sup>1</sup>, [Yanyu Li](https://scholar.google.com/citations?user=XUj8koUAAAAJ&hl=en)<sup>1</sup>,   
[Dahua Lin](http://dahua.site/)<sup>2</sup>, [Xihui Liu](https://xh-liu.github.io/)<sup>3</sup>, [Ziwei Liu](https://liuziwei7.github.io/)<sup>4</sup>, [Sergey Tulyakov](http://www.stulyakov.com/)<sup>1</sup>.  
<sup>1</sup>Snap Inc.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<sup>2</sup>CUHK&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<sup>3</sup>HKU&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<sup>4</sup>NTU     

### [Project](https://snap-research.github.io/HyperHuman/) | [Paper](https://snap-research.github.io/HyperHuman/content/hyperhuman.pdf) | [arXiv](https://arxiv.org/abs/2310.08579) | [Short Demo (3min)](https://www.youtube.com/watch?v=eRPZW1pwxog) | [Long Demo (10min)](https://www.youtube.com/watch?v=CxGfbwZOcyU)

Despite significant advances in large-scale text-to-image models, achieving hyper-realistic human image generation remains a desirable yet unsolved task. Existing models like Stable Diffusion and DALL·E 2 tend to generate human images with incoherent parts or unnatural poses. To tackle these challenges, our key insight is that human image is inherently structural over multiple granularities, from the coarse-level body skeleton to fine-grained spatial geometry. Therefore, capturing such correlations between the explicit appearance and latent structure in one model is essential to generate coherent and natural human images. To this end, we propose a unified framework, **HyperHuman**, that generates in-the-wild human images of high realism and diverse layouts. Specifically, **1)** we first build a large-scale human-centric dataset, named *HumanVerse*, which consists of 340M images with comprehensive annotations like human pose, depth, and surface normal. **2)** Next, we propose a *Latent Structural Diffusion Model* that simultaneously denoises the depth and surface normal along with the synthesized RGB image. Our model enforces the joint learning of image appearance, spatial relationship, and geometry in a unified network, where each branch in the model complements to each other with both structural awareness and textural richness. **3)** Finally, to further boost the visual quality, we propose a *Structure-Guided Refiner* to compose the predicted conditions for more detailed generation of higher resolution. Extensive experiments demonstrate that our framework yields the state-of-the-art performance, generating hyper-realistic human images under diverse scenarios.

<img src='./content/teaser.png' width=800>

## Citation

If you find our work useful, please kindly cite as:
```
@article{liu2023hyperhuman,
    title={HyperHuman: Hyper-Realistic Human Generation with Latent Structural Diffusion},
    author={Liu, Xian and Ren, Jian and Siarohin, Aliaksandr and Skorokhodov, Ivan and Li, Yanyu and Lin, Dahua and Liu, Xihui and Liu, Ziwei and Tulyakov, Sergey},
    journal={arXiv preprint arXiv:2310.08579},
    year={2023}
}
```

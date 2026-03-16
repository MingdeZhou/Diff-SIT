
# Efficient Video Diffusion with Sparse Information Transmission for Video Compression
[Zheng Chen](https://zheng-chen.cn), [Mingde Zhou](https://orcid.org/0009-0003-6642-7349), and [Yulun Zhang](http://yulunzhang.com/), "Efficient Video Diffusion with Sparse Information Transmission for Video Compression"

<div>
<a href="https://github.com/z-z-zmd/Diff-SIT/releases" target='_blank' style="text-decoration: none;"><img src="https://img.shields.io/github/downloads/z-z-zmd/Diff-SIT/total?color=green&style=flat"></a>
<a href="https://github.com/z-z-zmd/Diff-SIT" target='_blank' style="text-decoration: none;"><img src="https://visitor-badge.laobi.icu/badge?page_id=z-z-zmd/Diff-SIT"></a>
<a href="https://github.com/z-z-zmd/Diff-SIT" target='_blank' style="text-decoration: none;"><img src="https://img.shields.io/github/stars/z-z-zmd/Diff-SIT?style=social"></a>
</div>


[[project]()] [[arXiv]()] [[supplementary material]()] [dataset] [pretrained models]



#### 🔥🔥🔥 News

- **2026-3-16:** This repo is released.

---

> **Abstract:** Video compression aims to maximize reconstruction quality with minimal bitrates. Beyond standard distortion metrics, perceptual quality and temporal consistency are also critical. However, at ultra-low bitrates, traditional end-to-end compression models tend to produce blurry images of poor perceptual quality. Besides, existing generative compression methods often treat video frames independently and show limitations in time coherence and efficiency. To address these challenges, we propose the Efficient Video \textbf{Diff}usion with \textbf{S}parse \textbf{I}nformation \textbf{T}ransmission (Diff-SIT), which comprises the Sparse Temporal Encoding Module (STEM) and the One-Step Video Diffusion with Frame Type Embedder (ODFTE). The STEM sparsely encodes the original frame sequence into an information-rich intermediate sequence, achieving significant bitrate savings. Subsequently, the ODFTE processes this intermediate sequence as a whole, which exploits the temporal correlation. During this process, our proposed Frame Type Embedder (FTE) guides the diffusion model to perform adaptive reconstruction according to different frame types to optimize the overall quality. Extensive experiments demonstrate that Diff-SIT establishes a new state-of-the-art in perceptual quality and temporal consistency, particularly in the challenging ultra-low-bitrate regime.


### Pipeline

![](image/Architecture.png)

---

### Performance

<img src="image/bubble.png">

## 🔖 TODO

- [ ] Release testing and training code.
- [ ] Release pre-trained models.
- [ ] Provide WebUI.
- [ ] Provide HuggingFace demo.

## 🔗 Contents

1. Datasets
1. Models
1. Training
1. Testing
1. [Results](#results)
1. [Acknowledgements](#acknowledgements)

## <a name="results"></a>🔎 Results

We achieve impressive performance on image compression tasks.

<details open>
<summary>Quantitative Results (click to expand)</summary>

- Results in Fig. 4 of the main paper

<p align="center">
  <img width="900" src="figs/result_Fig4.png">
</p>
</details>

<details open>
<summary>Qualitative Results (click to expand)</summary>

- Results in Fig. 5 of the main paper

<p align="center">
  <img width="900" src="figs/result_Fig5.png">
</p>
<details>
<summary>More Qualitative Results</summary>

- Rate-Distortion-Perception Results (Fig. 4 of the supplementary material)

<p align="center">
  <img width="900" src="figs/more_results4.png">
</p>

- Visual Comparison Results (Fig. 5 of the supplementary material)

<p align="center">
  <img width="900" src="figs/more_results3.png">
</p>

- Extended Qualitative Results (Fig. 6 of the supplementary material)

<p align="center">
  <img width="900" src="figs/more_results5.png">
</p>

- Additional Results on DIV2K-val (Fig. 7 of the supplementary material)

<p align="center">
  <img width="900" src="figs/more_results1.png">
</p>

- Additional Results on Kodak (Fig. 7 of the supplementary material)

<p align="center">
  <img width="900" src="figs/more_results2.png">
</p>
</details>

</details>

## <a name="citation"></a>📎 Citation

If you find the code helpful in your research or work, please cite the following paper(s).

```
@inproceedings{chen2026steering,
  title={Steering One-Step Diffusion Model with Fidelity-Rich Decoder for Fast Image Compression},
  author={Chen, Zheng and Zhou, Mingde and Guo, Jinpei and Yuan, Jiale and Ji, Yifei and Zhang, Yulun},
  booktitle={AAAI},
  year={2026}
}
```

## <a name="acknowledgements"></a>💡 Acknowledgements

This project is based on [HiFiC](https://github.com/Justin-Tan/high-fidelity-generative-compression) and [OSEDiff](https://github.com/cswry/OSEDiff).


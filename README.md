# FuxiTranyu: A Multilingual Large Language Model Trained with Balanced Data
FuxiTranyu-8B is an **open-source** **multilingual large language model** trained from scratch, with a specific focus on the multilinguality. It is trained on 600B tokens with a balanced data distribution across languages, exhibiting remarkable multilingual performance compared to previous multilingual LLMs like BLOOM-7B, PolyLM-13B. 

FuxiTranyu supports 43 natural languages (Arabic, Bengali, Bulgarian, Burmese, Catalan, Chinese, Czech, Dutch, English, Filipino, Finnish, French, German, Greek, Hebrew, Hindi, Hungarian, Indonesian, Italian, Japanese, Kazakh, Khmer, Korean, Kurdish, Kyrgyz, Lao, Malay, Persian, Polish, Portuguese, Romanian, Russian, Spanish, Swedish, Tamil, Tajik, Thai, Turkish, Turkmen, Ukrainian, Urdu, Uzbek, and Vietnamese) and cover 16 programming languages (Java, JavaScript, Python, PHP, C, C++, C#, TypeScript, Go, SQL, Rust, Ruby, Scala, Lua, Assembly, and Visual Basic).

More details on the data collection & processing, pretraining and fine-tuning of FuxiTranyu can be found in the [technical report](https://arxiv.org/abs/2408.06273).

In addition to the base model and its checkpoints, we also release two instruction-tuned variants: SFT version and DPO version.

<div align="center">
<a href="https://huggingface.co/TJUNLP/FuxiTranyu-8B" target="_blank">
    <img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-FuxiTranyu-ffc107?color=ffc107&logoColor=white"/></a> <a href="https://huggingface.co/TJUNLP/FuxiTranyu-8B-SFT" target="_blank">
    <img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-FuxiTranyu%20SFT-ffc107?color=ffc107&logoColor=white" /></a> <a href="https://huggingface.co/TJUNLP/FuxiTranyu-8B-Chat" target="_blank">
    <img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-FuxiTranyu%20Chat-ffc107?color=ffc107&logoColor=white"/></a>
</div>
<div align='center'>
  <a href="https://arxiv.org/abs/2408" target="_blank">
    <img alt="Arxiv" src="https://img.shields.io/badge/Arxiv-FuxiTranyu-7289da?logo=arxiv&logoColor=red&color=red" /></a>
  <a href="https://tjunlp-lab.github.io/" target="_blank">
    <img alt="Github" src="https://img.shields.io/badge/Github-TJUNLP-7289da?logo=github&logoColor=black&color=black" /></a>
</div>


## Evaluation Results

We have evaluated FuxiTranyu-8B models on various multilingual benchmarks. Main results are shown as follows.  

|               | Multilingual ARC | Multilingual HellaSwag | XWinograd | XStoryCloze | XCopa |
| ------------- | ---------------- | ---------------------- | --------- | ----------- | ----- |
| BLOOM-7B      | 31.8             | 43.4                   | 70.0      | 58.2        | 56.9  |
| PolyLM-13B    | 30.6             | 46.0                   | 73.4      | 56.4        | 58.9  |
| Llama-2-7B    | 35.5             | 48.6                   | 78.0      | 55.6        | 56.7  |
| FuxiTranyu-8B | 32.7             | 51.8                   | 76.1      | 58.9        | 60.5  |

|                        | Multilingual ARC | Multilingual HellaSwag | Xwinograd | XStoryCloze | XCopa | Translation | XLSum |
| ---------------------- | ---------------- | ---------------------- | --------- | ----------- | ----- | ----------- | ----- |
| BLOOMZ-7B1             | 31.2             | 38.0                   | 64.0      | 49.8        | 53.3  | 14.7        | 4.4   |
| PolyLM-MultiAlpaca-13B | 28.6             | 39.1                   | 70.9      | 57.0        | 59.9  | -           | -     |
| Llama-2-7B-Chat        | 36.4             | 46.3                   | 74.8      | 56.5        | 55.9  | 22.1        | 4.6   |
| FuxiTranyu-8B-SFT      | 31.8             | 51.5                   | 75.7      | 56.6        | 61.3  | 25.9        | 8.9   |
| FuxiTranyu-8B-DPO      | 32.8             | 52.2                   | 74.1      | 56.9        | 62.1  | 26.4        | 7.3   |

More details of the performance on the specific language can be found at the technical report.

## Available Model Checkpoints

We release the FuxiTranyu-8B models, e.g., FuxiTranyu-8B, FuxiTranyu-8B-SFT, and FuxiTranyu-8B-DPO on the Hugging Face pages. To support a broader research on the multilingual LLM, we also release the intermedia checkpoints of the FuxiTranyu-8B model.

| Model             | Download                                                     |
| ----------------- | ------------------------------------------------------------ |
| FuxiTranyu-8B     | 🤗 [TJUNLP/FuxiTranyu-8B](https://huggingface.co/TJUNLP/FuxiTranyu-8B) |
| FuxiTranyu-8B-SFT | 🤗 [TJUNLP/FuxiTranyu-8B-SFT](https://huggingface.co/TJUNLP/FuxiTranyu-8B-SFT) |
| FuxiTranyu-8B-DPO | 🤗 [TJUNLP/FuxiTranyu-8B-DPO](https://huggingface.co/TJUNLP/FuxiTranyu-8B-DPO) |

## License

FuxiTranyu-8B models are under the apache-2.0 license.

## Citation

```bibtex
@article{FuxiTranyu8B,
      title={FuxiTranyu: A Multilingual Large Language Model Trained with Balanced Data}, 
      author={Haoran Sun, Renren Jin, Shaoyang Xu, Leiyu Pan, Supryadi, Menglong Cui, Jiangcun Du, Yikun Lei, Lei Yang, Ling Shi, Juesi Xiao, Shaolin Zhu, and Deyi Xiong},
      journal={arxiv preprint arXiv:2408.06273},
      year={2024},
      url={https://arxiv.org/abs/2408.06273}
}
```

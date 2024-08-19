<p align="center">
<h1 align="center"> <img src="images/hobby.png" alt="PNG Image" width="25" height="25"> Multimodal Causal Reasoning Benchmark: Challenging Vision Large Language Models to Infer Causal Links Between Siamese Images</h1>
</p>

<div align="center">

[**Zhiyuan Li**](https://github.com/Zhiyuan-Li-John)<sup></sup> · [**Heng Wang**](https://scholar.google.com.au/citations?user=jPj4ViQAAAAJ&hl=en&oi=ao)<sup></sup> · [**Dongnan Liu**](https://scholar.google.com.au/citations?user=JZzb8XUAAAAJ&hl=en&oi=ao)<sup></sup> · [**Chaoyi Zhang**](https://scholar.google.com.au/citations?user=GSM6eT0AAAAJ&hl=en&oi=ao)<sup></sup> · [**Ao Ma**] · [**Jieting Long**]  · [**Weidong Cai**](https://scholar.google.com.au/citations?user=N8qTc2AAAAAJ&hl=en&oi=ao)<sup></sup>

<sup>1</sup>University of Sydney

<a href='https://'><img src='https://img.shields.io/badge/Project-Page-green'></a>
<a href='https://'><img src='https://img.shields.io/badge/Arxiv-Paper-red'></a>
<a href='https://'><img src='https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue'></a>
</div>

<p align="center">
  	<b>
    [<a href="https://">ArXiv</a>] | [<a href="https://">🤗HuggingFace</a>] | [<a href="https://">Website</a>]
    </b>
    <br />
</p>

MuCR is proposed to challenge VLLMs to infer semantic cause-and-effect relationships when solely relying on visual cues such as action, appearance, clothing, and environment.

<img src='images/picture3.png'>

## Release
- [2024/08/15] 🔥 We release the [complete dataset](https://).
- [2024/08/15] 🔥 We release the [arxiv paper](https://).
- [2024/08/15] 🔥 We launch the [project page](https://).

## Demos

### Overview

<p align="center">
  <img src="images/Picture6.png">
</p>

### Model Performance

<p align="center">
  <img src="images/performance.png">
</p>

### Detailed Examples

<p align="center">
  <img src="images/human2.png" alt="Image 1" style="display: inline-block;">
  <img src="images/animal3.png" alt="Image 2" style="display: inline-block;">
  <img src="images/plant4.png" alt="Image 3" style="display: inline-block;">
  <img src="images/character5.png" alt="Image 4" style="display: inline-block;">
  <img src="images/mixture6.png" alt="Image 6" style="display: inline-block;">
</p>

## Download

You can directly download the model from [Huggingface](https://).
or load dataset from Huggingface as follows:
```python 
import datasets
dataset = datasets.load_dataset("data/")
```
## Dataset Form
Each line of file in `jsonl` must meet the following format:
```json
{
  "id": "ID",
  "caption_0": "...",
  "caption_1": "...",
  "link_id": "[a,b,c]",
  "cue": "cue",
  "false_cue": ["false_cue1","false_cue2","flase_cue3"],
  "style": "style",
  "label": "label",
  "causal_reason": ["Explanation_1", "Explanation_2", "Explanation_3"]
}
```

## Reference
If you find this project useful for your research, please consider citing the following paper:

```
@inproceedings{
}
```

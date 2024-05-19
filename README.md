# StyleTalk Dataset 🗣

* Speech-to-speech conversation with speaking styles
* Varied emotions, speaking speeds, speaking volumes
* Human-annotated filtering
* Read more details in [paper](https://arxiv.org/abs/2402.12786) (ACL 2024 main conference paper)
<img width="500" alt="image" src="https://github.com/DanielLin94144/StyleTalk/assets/50494525/4416a3fe-7c8c-4bab-8b4e-77685b7afcbe">


## Introduction
In spoken dialogue, even if two current turns are the same sentence, their responses might still differ when they are spoken in different styles. The spoken styles, containing paralinguistic and prosodic information, mark the most significant difference between text and speech modality. When using text-only LLMs to model spoken dialogue, text-only LLMs cannot give different responses based on the speaking style of the current turn. In this paper, we focus on enabling LLMs to listen to the speaking styles and respond properly. Our goal is to teach the LLM that "even if the sentences are identical if they are spoken in different styles, their corresponding responses might be different". Since there is no suitable dataset for achieving this goal, we collect a speech-to-speech dataset, StyleTalk, with the following desired characteristics: when two current speeches have the same content but are spoken in different styles, their responses will be different. To teach LLMs to understand and respond properly to the speaking styles, we propose the Spoken-LLM framework that can model the linguistic content and the speaking styles. We train Spoken-LLM using the StyleTalk dataset and devise a two-stage training pipeline to help the Spoken-LLM better learn the speaking styles. Based on extensive experiments, we show that Spoken-LLM outperforms text-only baselines and prior speech LLMs methods.

## Data
* Annotation file: ```train.csv``` and ```eval.csv```
* Audio files: [Google drive](https://drive.google.com/file/d/1y8L5BATyr8go0L-9DfIKtMek51koSlhp/view?usp=sharing)

## Spoken-LLM Framework
TBA

<img width="500" alt="image" src="https://github.com/DanielLin94144/StyleTalk/assets/50494525/bf15631a-d60d-4878-bc28-4bfa8470026f">

## Citation
If you use the dataset or find the paper useful for your research, please cite the paper: 
```
@article{lin2024advancing,
  title={Advancing Large Language Models to Capture Varied Speaking Styles and Respond Properly in Spoken Conversations},
  author={Lin, Guan-Ting and Chiang, Cheng-Han and Lee, Hung-yi},
  journal={arXiv preprint arXiv:2402.12786},
  year={2024}
}
```

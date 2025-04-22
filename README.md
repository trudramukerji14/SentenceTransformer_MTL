Here we implement the sentence transformer DistilBERT a lightweight version of BERT and use it as the transformer backbone for multi-task learning. 


<p align="center">
  <img src="https://github.com/trudramukerji14/SentenceTransformer_MTL/blob/main/images/BERT_embeddings_01.png" height="250" alt="AskVideos-VideoCLIP" />
</p>
<p align="center">
  <em>High-level schematic diagram of BERT (taken from Wikipedia).</em>
</p>
<p align="center">
    <a href='https://huggingface.co/papers/1910.01108'><img src='https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Checkpoint-blue'></a>
    <a target="_blank" href="https://colab.research.google.com/drive/1E-Pi_kbkLe6qtk4q_fn0UYsie93BWJPF?usp=sharing">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
    </a>
</p>
<p align="center">
  
## Motivation

Many NLP tasks share underyling language understanding for various tasks. By implementing and training a model on different tasks, allows the model to share parameters and benefit from a potentially richer understanding.

(Recommended): The notebook is available to run on colab, one can access it by simply clicking on the "Open in Colab" button above.

## Summary

In this project, we build a multi-task model for the tasks of detecting food keywords and sentiment analysis and write a function to train it on [yelp review](https://huggingface.co/datasets/Yelp/yelp_review_full) dataset available in HuggingFace. 

Namely, in this project we execute four tasks:

- **Task 1**: Implement a Sentence Transformer and run it on some sample sentences.
- **Task 2**: Write the class for the multitask model.
- **Task 3**: Discuss various training considerations and freezing various parameters.
- **Task 4**: Implement a training function for the model.

## Usage

#### Environment Preparation
First, create a conda environment:
```
conda create my_env python=3.9 
conda activate my_env
```
Then, install the requirements:
```
pip3 install -U pip
pip3 install -r requirements.txt
```

## How to Run Demo Locally
One can run the .py file in the notebook subfolder as follows. 
```
python sentencetransformer_multitask.py 
```

## Repository Structure

The notebooks folder contains the .ipynb file and the .py file (where the markdown and tensorboard is converted to comments)






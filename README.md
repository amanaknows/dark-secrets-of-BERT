# Introduction
For installation and usage please refer to [release 0.6 of pytorch_pretrained_bert](https://github.com/huggingface/transformers/releases).

The current fork adds the attention analysis of 12 layer BERT. For details please refer to [the paper](https://arxiv.org/abs/1908.08593).

# Usage
1. Install the requirements as
```
pip install -r requirements.txt
```

2. The current implementation assumes you have fine-tuned BERT model weights saved to a directory of your choice. 

3. The code for analysis is contained in [the jupyter notebook](./visualize_attention.ipynb).

4. 


# References
```
@article{kovaleva2019revealing,
  title={Revealing the Dark Secrets of BERT},
  author={Kovaleva, Olga and Romanov, Alexey and Rogers, Anna and Rumshisky, Anna},
  journal={arXiv preprint arXiv:1908.08593},
  year={2019}
}
```


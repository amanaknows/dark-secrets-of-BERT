# Introduction
For installation and docs please refer to [release 0.6 of pytorch_pretrained_bert](https://github.com/huggingface/transformers/releases).

The current fork adds the jupyter notebook on the attention analysis of the 12 layer BERT model. For details please refer to [the paper](https://arxiv.org/abs/1908.08593).

Note that for the extraction of attention weights the source code of [](./pytorch_pretrained_bert/modeling.py) was modified (this functionality was added in later realeases of the forked repo).

# Requirements and usage
1. Install the requirements as
```
pip install -r requirements.txt
```

2. The current implementation assumes you have GLUE datasets downloaded and fine-tuned BERT model weights saved to a directory of your choice. You can download GLUE data as described [here](https://github.com/nyu-mll/GLUE-baselines/blob/master/download_glue_data.py). To fine-tune BERT, run [](./examples/run_classifier.py).

3. The code for analysis is contained in [the jupyter notebook](./visualize_attention.ipynb). 

4. To repeat the results of experiments, make sure to change the `path_to_model` and `path_to_data` in the notebook.


# References
```
@article{kovaleva2019revealing,
  title={Revealing the Dark Secrets of BERT},
  author={Kovaleva, Olga and Romanov, Alexey and Rogers, Anna and Rumshisky, Anna},
  journal={arXiv preprint arXiv:1908.08593},
  year={2019}
}
```


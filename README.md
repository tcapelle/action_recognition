# Action Recognition
> Implementation of various architectures to solve the UCF 101 actions dataset


It is based on the implementations found on [Action Recognition](https://github.com/eriklindernoren/Action-Recognition).

I try to keep with updated architectures that come out. Right now transformers are all we need... Follow @lucidrains to get the next attention based model ASAP.

## Install

First install `fastai`:
```bash
$ pip install fastcore fastai
```

## Results
Results are computed on a random splut 80%/20%. Using `fastai2` built-in `fit_one_cycle` training.

- [train baseline](01_train_baseline.ipynb): Implements a Basic Resnet 34 encoder coupled with a simple attention layer over the frames. (91% accuracy)
- [train convlstm](02_train_convlstm.ipynb): resnet34 encoder + LSTM layer over image features. (84.8% accuracy)
- [train_transformer](03_train_transformer.ipynb): Added the new TimeSformer and STAM from @lucidrains implementations.

This package also provides function to download nad process the video dataset into multiple frames.

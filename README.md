# Action Recognition
> Implementation of various architectures to solve the UCF 101 actions dataset


This repo implementation is using `fastai` library (version 2). It is based on the implementations found on [Action Recognition](https://github.com/eriklindernoren/Action-Recognition).

## Install

First install `fastai`: (version 2, it has been released)
```bash
$ pip install fastcore fastai
```

then clone the repo, and inside the repo's folder do:

```bash
$ pip install -e .
```

## Results
Results are computed on a random splut 80%/20%. Using `fastai2` built-in `fit_one_cycle` training.

- [train baseline](nbs/04_train_baseline.ipynb): Implements a Basic Resnet 34 encoder coupled with a simple attention layer over the frames. (91% accuracy)
- [train convlstm](nbs/04_train_convlstm.ipynb): resnet34 encoder + LSTM layer over image features. (84.8% accuracy)
- [train_transformer](nbs/05_train_transformer.ipynb): Added the new TimeSformer ~~Transformer based model, inspired from DETR. This is in early stages, only supporting batch size equal to 1.~~

This package also provides function to download nad process the video dataset into multiple frames.

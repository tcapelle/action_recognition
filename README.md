# Action Recognition
> Implementation of various architectures to solve the UCF 101 actions dataset


This repo is based on `fastai2` library. It is based on the implementations found on [Action Recognition](https://github.com/eriklindernoren/Action-Recognition).

## Install

First install `fastai2`:
```bash
$ pip install fastcore fastai2
```

You have to first clone the repo, and then inside the repo's folder do:

```bash
$ pip install -e .
```

## Results

- [train baseline](nbs/04_train_baseline.ipynb): Implements a Basic Resnet 34 encoder coupled with a simple attention layer over the frames.
- [train convlstm](nbs/04_train_convlstm.ipynb): resnet34 encoder + LSTM layer over image features.

This package also provides function to download nad process the video dataset into multiple frames, check [utils notebooks](nbs/01_utils.ipynb)

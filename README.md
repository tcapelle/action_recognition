# Action Recognition
> Implementation of various architectures to solve the UCF 101 actions dataset


This repo implementation is using `fastai2` library. It is based on the implementations found on [Action Recognition](https://github.com/eriklindernoren/Action-Recognition).

## Install

First install `fastai2`:
```bash
$ pip install fastcore fastai2
```

then clone the repo, and inside the repo's folder do:

```bash
$ pip install -e .
```

## Results

- [train baseline](nbs/04_train_baseline.ipynb): Implements a Basic Resnet 34 encoder coupled with a simple attention layer over the frames. (91.7% accuracy)
- [train convlstm](nbs/04_train_convlstm.ipynb): resnet34 encoder + LSTM layer over image features. (94.8% accuracy)

This package also provides function to download nad process the video dataset into multiple frames, check [utils notebooks](nbs/01_utils.ipynb).

I am actually at home doing everythin on a small laptop with a GTX 1050 mobile GPU, so I am very limited to do proper benchmark.

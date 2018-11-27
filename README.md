# AdaNet

[![PyPI version](https://badge.fury.io/py/adanet.svg)](https://badge.fury.io/py/adanet)
[![Travis](https://travis-ci.org/tensorflow/adanet.svg?branch=master)](https://travis-ci.org/tensorflow/adanet)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/tensorflow/adanet/blob/master/LICENSE)

<div align="center">
  <img src="https://tensorflow.github.io/adanet/images/adanet_tangram_logo.png" alt="adanet_tangram_logo"><br><br>
</div>

**AdaNet** is a lightweight and scalable TensorFlow AutoML framework for training and deploying adaptive neural networks using the *AdaNet* algorithm [[Cortes et al. ICML 2017](https://arxiv.org/abs/1607.01097)]. *AdaNet* combines several learned subnetworks in order to mitigate the complexity inherent in designing effective neural networks.

<div align="center" style="max-width: 450px; display: block; margin: 0 auto;">
  <img src="https://tensorflow.github.io/adanet/images/adanet_animation.gif" alt="adanet_tangram_logo" style="max-height: 450px;"><br><br>
</div>

This is not an official Google product.

## Getting Started

To get you started:

- [Tutorials: for understanding the AdaNet algorithm and learning to use this package](./adanet/examples/tutorials)

## Requirements

Requires [Python](https://www.python.org/) 2.7, 3.4, 3.5, or 3.6.

`adanet` depends on bug fixes and enhancements not present in TensorFlow releases prior to 1.9. You must install or upgrade your TensorFlow package to at least 1.9:

```shell
$ pip install "tensorflow>=1.9.0"
```

## Installing with Pip

You can use the [pip package manager](https://pip.pypa.io/en/stable/installing/) to install the official `adanet` package from [PyPi](https://pypi.org/project/adanet/):

```shell
$ pip install adanet
```

## Installing from source

To install from source first you'll need to install `bazel` following their [installation instructions](https://docs.bazel.build/versions/master/install.html).

Next clone `adanet` and `cd` into its root directory:

```shell
$ git clone https://github.com/tensorflow/adanet && cd adanet
```

From the `adanet` root directory run the tests:

```shell
$ cd adanet
$ bazel test -c opt //...
```

Once you have verified that everything works well, install `adanet` as a [ pip package ](./adanet/pip_package/PIP.md).

You are now ready to experiment with `adanet`.

```python
import adanet
```

## License

AdaNet is released under the [Apache License 2.0](LICENSE).

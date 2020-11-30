# MLModelScope Caffe Agent

[![Go Report Card](https://goreportcard.com/badge/github.com/c3sr/caffe)](https://goreportcard.com/report/github.com/c3sr/caffe)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)


This is the Caffe agent for [MLModelScope](mlmodelscope.org), an open-source framework and hardware agnostic, extensible and customizable platform for evaluating and profiling ML models across datasets / frameworks / systems, and within AI application pipelines.

Currently it has most of the vison models from [Caffe Model Zoo](https://github.com/BVLC/caffe/wiki/Model-Zoo) built in. More built-in models are comming.
One can evaluate the **~40** models on any systems of insterest with either local Caffe installation or Caffe docker images.

Check out [MLModelScope](mlmodelscope.org) and welcome to contribute.


## Installation

Install go if you have not done so. Please follow [Go Installation](https://docs.mlmodelscope.org/installation/source/golang).

Download and install the MLModelScope Caffe Agent:

```
go get -v github.com/c3sr/caffe

```

The agent requires The Caffe C library and other Go packages.

### Go packages

You can install the dependency through `go get`.

```
cd $GOPATH/src/github.com/c3sr/caffe
go get -u -v ./...
```

Or use [Dep](https://github.com/golang/dep).

```
dep ensure -v
```

This installs the dependency in `vendor/`.

Note: The CGO interface passes go pointers to the C API. This is an error by the CGO runtime. Disable the error by placing

```
export GODEBUG=cgocheck=0
```

in your `~/.bashrc` or `~/.zshrc` file and then run either `source ~/.bashrc` or `source ~/.zshrc`


### The Caffe C library

The Caffe C library is required.

If you use Caffe Docker Images (e.g. NVIDIA GPU CLOUD (NGC)), skip this step.

Refer to [go-caffe](https://github.com/c3sr/go-caffe#caffe-installation) for caffe installation.


## External services

Refer to [External services](https://github.com/c3sr/tensorflow#external-services).

## Use within Caffe Docker Images

Refer to [Use within TensorFlow Docker Images](https://github.com/c3sr/tensorflow#use-within-tensorflow-docker-images).

## Usage

Refer to [Usage](https://github.com/c3sr/tensorflow#usage)

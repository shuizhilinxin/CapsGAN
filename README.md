# CapsGAN 
Unsupervised representation learning with CapsNet based Generative Adversarial Networks


## Description

Coalesces Wassertein Distance algorithm based generative adversarial networks with deep convolutinal network based discriminator replaced by CapsNet architecture.

## Prerequisits and Requirements

* Python > 3.6
* PyTorch
* TorchVision
* TorchNet
* TQDM
* Visdom [_optional_]

** For training, an NVIDIA TITAN XP GPU was used. __Using CUDA with GPU is strongly recommended__. CPU is supported but speed of training will be very slow.

## Datasets

* MNIST
* CIFAR-10

## Usage

Utilizes FAIR's visdom as visulization tool. If you'd like to visualize the test and train results, run with `visualize` args. 

```bash
$ sudo python3 -m visdom.server &
$ python3 main.py --visualize --cuda
```

Else, simply run:

```bash
$ python3 main.py --dataset cifar10 --dataroot ./data --cuda --niter [NUM_EPOCHS] --
```

To run with MLP as G or D, run:
```bash
$ python3 main.py --dataset cifar10 --dataroot ./data --cuda --experiment {Name} --mlp_G --ngf 512
```

## Contact
Please send an email to raeidsaqur[at]cs[dot]toronto[dot]edu for questions, PRs etc.

*** Note: __Improved ReadMe is in the works!__ 






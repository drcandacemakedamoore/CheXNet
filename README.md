# CheXNet for Classification and Localization of Thoracic Diseases
This is a fork of a Pytorch meant to customize it for my own purposes. Please see other versions of the project to customize it for your needs. 

This is a Python3 (Pytorch) reimplementation of [CheXNet](https://stanfordmlgroup.github.io/projects/chexnet/). The model takes a chest X-ray image as input and outputs the probability of certain thoracic pathologies along with a likelihood map of pathologies.

<div align=center><img width="500" height="500" src="./localization/00008473_011-3.png"/></div>

## Dataset

The original dataset for the original project:

The [ChestX-ray14 dataset](http://openaccess.thecvf.com/content_cvpr_2017/papers/Wang_ChestX-ray8_Hospital-Scale_Chest_CVPR_2017_paper.pdf) comprises 112,120 frontal-view chest X-ray images of 30,805 unique patients with 14 disease labels. To evaluate the model, we randomly split the dataset into training (70%), validation (10%) and test (20%) sets, following the work in paper. Partitioned image names and corresponding labels are placed under the directory [labels](./ChestX-ray14/labels).

## Prerequisites

- Python 3.4+
- [PyTorch](http://pytorch.org/) and its dependencies

## Usage

0. I would clone a repository without my modifications...but if you want: 

1. Clone this repository.

2. Download images of ChestX-ray14 from this [released page](https://nihcc.app.box.com/v/ChestXray-NIHCC) and decompress them to the directory [images](./ChestX-ray14/images).

3. Specify one or multiple GPUs and run

   `python model.py`



## Contributions

This work is based on earllier work  collaboratively conducted by Xinyu Weng, Nan Zhuang, Jingjing Tian and Yingcheng Liu.
They were students/interns of Machine Intelligence Lab, Institute of Computer Science & Technology, Peking University, directed by Prof. Yadong Mu (http://www.muyadong.com).
They in tern based their work off the original CheXnet project out of Stanford.

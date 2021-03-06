# DoGNet
A Deep Architecture for Synapse Detection in Multiplexed Fluorescence Images

![Alt text](images/Pipeline2g.png?raw=true "DoGNet Pipeline")

We propose DoGNet, a neural architecture, that closes the gap between classical computer vision blob detectors, such as Difference of Gaussians (DoG) filters, and modern convolutional networks. DoGNet is optimized to take in highly multiplexed microscopy data. Due to small number of trainable parameters, DoGNet can be trained with only few examples, which facilitates application of the tool to new datasets and prevents overfitting. We evaluate our method on multiplexed fluorescence imaging data in both primary mouse neuronal cultures and mouse cortex tissue slices. We show that DoGNet outperforms convolutional networks with a low to moderate number of training examples. DoGNet synapse localizations are then used to guide the segmentation of individual synaptic protein locations and extent, revealing the spatial organization of proteins within synapses and their abundances.

## Requirements
* Python 2.7/3.6
* PyTorch (http://pytorch.org/)
* Numpy
* Scipy
* Scikit-image
* Sklearn
* Matplotlib

## GPU or CPU
* For inference GPU is not required (you can our pretrained models without GPU)
* For training GPU is strongly recomended


## Installation/Uninstall/Run
* python setup.py install --user
* pip uninstall dognet
* /run/run_prism.py or any other. results will be saved as csv to results folder
* using jupyter run any notebook from notebooks folder

## Installation on Windows
* install pytorch https://github.com/peterjc123/pytorch-scripts
* python setup.py install --user
* /run/run_prism.py or any other. results will be saved as csv to results folder

## Acknowledgements
This work is supported by Skoltech NGP Program (Skoltech-MIT joint project)

# BHViT
This code is an implementation of our work "BHViT: Binarized Hybrid Vision Transformer."

[Reference]: Tian Gao, Zhiyuan Zhang, Yu Zhang, Huajun Liu, Kaijie Yin, Chengzhong Xu, and Hui Kong, [BHViT: Binarized Hybrid Vision Transformer](https://arxiv.org/abs/2503.02394), IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2025


----------------------------------------------------------------------------------------------------------------------------------------------------------
# [BHViT: Binarized Hybrid Vision Transformer]()
### Introduction
Model binarization has made significant progress in enabling real-time and energy-efficient computation for convolutional neural networks (CNN), offering a potential solution to the deployment challenges faced by Vision Transformers (ViTs) on edge devices. However, due to the structural differences between CNN and Transformer architectures, simply applying binary CNN strategies to the ViT models will lead to a significant performance drop. To tackle this challenge, we propose BHViT, a binarization-friendly hybrid ViT architecture and its full binarization model with the guidance of three important observations. Initially, BHViT utilizes the local information interaction and hierarchical feature aggregation technique from coarse to fine levels to address redundant computations stemming from excessive tokens. Then, a novel module based on shift operations is proposed to enhance the performance of the binary Multilayer Perceptron (MLP) module without significantly increasing computational overhead. In addition, an innovative attention matrix binarization method based on quantization decomposition is proposed to evaluate the token's importance in the binarized attention matrix. Finally, we propose a regularization loss to address the inadequate optimization caused by the incompatibility between the weight oscillation in the binary layers and the Adam Optimizer. Extensive experimental results demonstrate that our proposed algorithm achieves SOTA performance among binary ViT methods.


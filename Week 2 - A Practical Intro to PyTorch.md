pytorch.org/tutorials/beginner/basics/intro

## Introduction
### What we need to train a NN
![](Pasted%20image%2020240515173649.png)
![](Pasted%20image%2020240515173804.png)

## Power of Frameworks
- Consistent
- Automates

## Pytorch v TensorFlow
- Overall the same now - used to be that pytorch was easy to get up and tensor flow was good for production
- Pytorch is more cutting edge - more pythonic
- ![](Pasted%20image%2020240515173925.png)
- ![](Pasted%20image%2020240515174154.png)
	- Multi-dimensional object

	- Documentation: https://pytorch.org/docs/stable/nn.html

# Layers
- Contain Tensors
- ![](Pasted%20image%2020240515175355.png)
- [Containers](https://pytorch.org/docs/stable/nn.html#containers)
- [Convolution Layers](https://pytorch.org/docs/stable/nn.html#convolution-layers)
- [Pooling layers](https://pytorch.org/docs/stable/nn.html#pooling-layers)
- [Padding Layers](https://pytorch.org/docs/stable/nn.html#padding-layers)
- [Non-linear Activations (weighted sum, nonlinearity)](https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity)
- [Non-linear Activations (other)](https://pytorch.org/docs/stable/nn.html#non-linear-activations-other)
- [Normalization Layers](https://pytorch.org/docs/stable/nn.html#normalization-layers)
- [Recurrent Layers](https://pytorch.org/docs/stable/nn.html#recurrent-layers)
- [Transformer Layers](https://pytorch.org/docs/stable/nn.html#transformer-layers)
- [Linear Layers](https://pytorch.org/docs/stable/nn.html#linear-layers)
- [Dropout Layers](https://pytorch.org/docs/stable/nn.html#dropout-layers)
- [Sparse Layers](https://pytorch.org/docs/stable/nn.html#sparse-layers)
- [Distance Functions](https://pytorch.org/docs/stable/nn.html#distance-functions)
- [Loss Functions](https://pytorch.org/docs/stable/nn.html#loss-functions)
- [Vision Layers](https://pytorch.org/docs/stable/nn.html#vision-layers)
- [Shuffle Layers](https://pytorch.org/docs/stable/nn.html#shuffle-layers)
- [DataParallel Layers (multi-GPU, distributed)](https://pytorch.org/docs/stable/nn.html#module-torch.nn.parallel)
- [Utilities](https://pytorch.org/docs/stable/nn.html#module-torch.nn.utils)
- [Quantized Functions](https://pytorch.org/docs/stable/nn.html#quantized-functions)
- [Lazy Modules Initialization](https://pytorch.org/docs/stable/nn.html#lazy-modules-initialization)
- A layer is not just the tensor, it is also the gradient. That is why you cannot switch back and forth to numpy from the tensor

![](Pasted%20image%2020240515180445.png)
- Relu turns everything less than 0 to 0
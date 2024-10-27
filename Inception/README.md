# Image Classification Using Inception Networks

The following repository contains an implementation of Inception Networks (GoogleNet). Inception Networks were first introduced by Google in their 2014 paper titled “Going Deeper with Convolutions.” At the core of Inception Networks lies the inception block, which allows multiple convolutional filters to operate in parallel, aiming to capture various levels of detail from the input. The architecture of the network is as follows:
  
![image](https://github.com/user-attachments/assets/a29de052-88da-4dbb-bd84-75965341c2ec)


# Model Architecture
Below is a diagram of the Inception Block:

![image](https://github.com/user-attachments/assets/ee3f803e-808f-4acb-928d-2256ce534f7a)

The code includes the following components:

1. Inception Block: The core element of Inception Networks, this block enables multiple convolutional filters of different sizes to operate in parallel on the same input. This approach allows the model to capture features at various levels of detail, from fine-grained textures to broader patterns, enhancing the network’s ability to understand complex visual information.   
2.	Convolutional Block: A fundamental building block of the network, the Convolutional Block performs convolution operations that extract spatial features from the input. It includes layers for convolution, activation functions, and batch normalization, which helps in maintaining stable and efficient training.
3.	Auxiliary Network: To assist the training process, an Auxiliary Network is added as an intermediate classifier. This component provides additional supervision, especially useful in deep networks where gradient vanishing may occur. It helps to improve convergence and model performance by allowing gradients to flow through the network more effectively.   
4.	Neural Network Architecture: The complete architecture integrates multiple Inception and Convolutional Blocks, creating a deep network that can effectively capture complex patterns in data. The architecture culminates in fully connected layers, which transform the learned features into final predictions.   
  

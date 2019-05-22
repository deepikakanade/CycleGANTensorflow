# CycleGAN

A TensorFlow implementation of CycleGAN for neuroimaging data. 

The CycleGAN model is used to convert Post-gadolinium enhanced MRI images into pre-gad MRI images. The main advantage of using CycleGAN is to eliminate the requirement of paired data. 

!(./helpers/img_translation.jpeg)

The network architecture can be described as follows:

!(./helpers/model.jpg)

The generator is formed by using ResNet block defined in models.py. resnet_block is a neural network layer which consists of two convolution layers where a residue of input is added to the output. 

!(./helpers/Resnet.jpg)

The losses used in CycleGAN architecture are:
- Generator Loss
- Discriminator Loss
- Cyclic Loss

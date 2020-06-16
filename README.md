# NOTE: IF YOU HAVING TROUBLE OPENING JUPYTER NOTEBOOKS PLEASE OPEN THE FOLLOWING LINKS
<b>DCGAN</b> : https://nbviewer.jupyter.org/github/aryanshu/GAN-/blob/master/DCGAN.ipynb
<br><b>GAN</b>   : https://nbviewer.jupyter.org/github/aryanshu/GAN-/blob/master/GAN.ipynb 

# Implementation of GANs and DCGANs using PyTorch
The Generative Adversarial Network and Deep Convolutional Generative Adversarial Networks implemented in this project was based on the paper "<a href="https://arxiv.org/abs/1406.2661">Generative Adversarial Networks<a>" by Goodfellow et al. and  "<a href="https://arxiv.org/abs/1511.06434">Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks<a>" by Soumith Chintala Respectively.

Apart from DCGAN there are many extension have been introduced in the past 2 to 3 years related to GANs , still it is most attention seeker area in Computer Vision or Deep learning in general.   

## GANs:
General adversarial networks and It's family of adverserial Networks(including DCGANs) are two neural networks competing against each other to create an output that closely resembles the input. These two networks — the generator and the discriminator— are playing adversarial roles. The generator network creates a new image from random noise based off of the input image. The random noise evolves from incoherent pixels to a coherent image with discernible forms in it because of how the discriminator told it to change. The discriminator network determines if the image is real or fake. The goal of the GAN is for the generator image to be so like the real image that it is able to trick the discriminator into thinking that the generated image is real. One of the most important features of GANs, is that the neural networks implemented in GANs use a number of parameters significantly smaller than the amount data used to train them. This forces the model to learn and internalize the most important features in the data so the model can generate them.

## Architecture:
<p align="center"><img width="80%" src="./images/GAN.png" /></p>

## DCGANs
It is an extension of GANs . It mainly composes of convolution layers without max pooling or fully connected layers. It uses convolutional stride and transposed convolution for the downsampling and the upsampling. The figure below is the network design for the generator.

<p align="center"><img width="80%" src="./images/DCGAN.png" /></p>



## RESULTS

All results are generated from the fixed noise vector.<br>
<b> Results on MNIST digit dataset:</b><br>
MNIST digit dataset is a large database of handwritten digits .There are about 6000 train image and 10000 test images.<br>


*Name* | *Time Taken* | *Epoch 1* | *Mid Epoch* | *Max Epoch* | *GIF*
:---: | :---: | :---: | :---: | :---: | :---: |
GAN | 12.35 mins | <img src = 'images/1(gan-digit).png' width ='230' height = '125px'> | <img src = 'images/50(mid).png' width ='230' height = '125px'> | <img src = 'images/100.png' width ='230' height = '125px'> | <img src = 'https://user-images.githubusercontent.com/48057022/68598461-dca31d80-04c4-11ea-85ee-74892314c93c.gif' width="230px" height = '125px'>
DCGAN | 34.6 mins  | <img src = 'images/1(digit-dcgan).png'  width ='230px' height = '125px'> | <img src = 'images/15.png'  width="230px" height= '125px'> | <img src = 'images/30.png' width ='230px' height = '125px'> | <img src = 'https://user-images.githubusercontent.com/48057022/68599041-dd887f00-04c5-11ea-925b-d00ff5785ce2.gif' width="230px" height = '125px'>

<b>Results on Fashion MNIST dataset:</b><br>
MNIST digit dataset is a large database of fashion clothing product , It contains 10 clothing cateogry porducts .There are about 60,000  images.<br>

*Name* | *Time Taken* | *Epoch 1* | *Mid Epoch* | *Max Epoch* | *GIF*
:---: | :---: | :---: | :---: | :---: | :---: |
GAN | 62.7 mins | <img src = 'images/1.png' width ='230' height = '125px'> | <img src = 'images/250.png' width ='230' height = '125px'> | <img src = 'images/500.png' width ='230' height = '125px'>| <img src = 'images/fashion_gan.gif' width="230px" height = '125px'>
DCGAN | 64.9 mins | <img src = 'images/1(dcgan).png' width ='230px' height = '125px'> | <img src = 'images/25.png' width ='230' height = '125px'> | <img src = 'images/50.png' width ='230px' height = '125px'> | <img src = 'images/Fashion_dcgan.gif' width="230px" height = '125px'>





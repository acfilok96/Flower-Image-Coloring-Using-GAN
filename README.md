# Flower-Image-Coloring-Using-GAN

There are many old photographs in the world that were taken with black and white cameras. As such, recolonizing these photos has become a somewhat niche and popular hobby. Until recently, current methods of recolorization have been to recolor them meticulously by hand. In this project, given a grayscale image as input, our neural network aims to create a realistic and plausible colorization of that image. In the end, we aim to create realistic images using this method. We hypothesize that by using a convolutional neural network, we will be able to achieve the aforementioned goal. Specifically, by using a fully connected resnet as a backbone for our model and taking the first greyscale layer of the CIELAB color space as input into our neural network, we were able to achieve mostly realistic colorizations of the images with some exceptions. In the future, we would like to turn this implementation into a Generative Adversarial Network by adding a discriminator to our model to get even better results.

The aim of this notebook is to generate coloured image, given a grayscale image as input. This notebook takes inspiration from End-to-End Conditional GAN based Architectures for Image Colourisation by Marc Gorriz Blanch, Marta Mrak, Alan F. Smeaton and Noel E. O'Connor.

For the training of the model I had to create this dataset, wherein gray scale images are taken as input and a and b components of LAB color space are taken as output.

I used the base Pix2Pix GAN model for image colourisation. And as stated by the authors of this paper, a fraction of the images generated were desaturated. To mitigate the lack of colourfulness, this model architecture was proposed.


Generated Video:- 

https://user-images.githubusercontent.com/88615645/234381635-2bf618d3-94eb-4739-a19e-92475a9f2573.mp4


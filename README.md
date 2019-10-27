# Image Rating Neural Network

[See pdf version here](Image_Rater_Transfer_Learning.pdf).

Builds and trains a neural network that assigns aesthetic quality scores to images similarly to the general public. It is trained on images from the [AVA (Aesthetic Visual Analysis) dataset](http://refbase.cvc.uab.es/files/MMP2012a.pdf), available [here](http://academictorrents.com/details/71631f83b11d3d79d8f84efe0a7e12f0ac001460).

It first uses the [VGG19](https://github.com/machrisaa/tensorflow-vgg) network to convert images from the AVA dataset into codes, then runs the codes through a fully-connected network with two hidden layers, to return image ratings. The rating for an image is in the form of a probability distribution over the integers from 1 (lowest quality) to 10 (highest quality).

The ipynb is a file you can run on your computer using Jupyter Notebook. If you run the notebook, you will need the AVA dataset on your local computer. Note the hardcoded location ("E:/AVA_dataset") in the python code.

# Convolutional Neural Network (CNN)

for the previous example, while there are only 784 pixels, it will be interesting to see if there was a way that we could condense the image down to the important features that distinguish what makes it a shoe, or a handbag, or a shirt. 

## Convolution 

it usually involves having a filter and passing that filter over the image in order to change the underlying image. 

For every pixel, take its value, and take a look at the value of its neighbors. If our filter is three by three, then we can take a look at the immediate neighbor, so that you have a corresponding three by three grid.

new value for the pixel, we simply multiply each neighbor by the corresponding value in the FILTER.

so new pixel is obtained and thats convolution.

The idea here is that some convolutions will change the image in such a way that certain features in the image get emphasized.

## Pooling

Convolution with pooling is really powerful.

Pooling is a way of compressing an image.

Go over the image of four pixels at a time, i.e, the current pixel and its neighbors underneath and to the right of it. Of these four, pick the biggest value and keep just that.  This will preserve the features that were highlighted by the convolution, while simultaneously quartering the size of the image. We have the horizontal and vertical axes.

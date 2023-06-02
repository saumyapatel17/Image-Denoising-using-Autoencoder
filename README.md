# Image-Denoising-using-Autoencoder

This  project demonstrates how to implement a deep convolutional autoencoder for image denoising, mapping noisy digits images from the MNIST dataset to clean digits images. This implementation is based on an original blog post titled Building Autoencoders in Keras by François Chollet.

**Overview of Encoder-Decoder Network (Autoencoders)**

Autoencoder is an unsupervised artificial neural network that is trained to copy its input to output. In the case of image data, the autoencoder will first encode the image into a lower-dimensional representation, then decodes that representation back to the image. Encoder-Decoder automatically consists of the following two structures:

* The encoder- This network downsamples the data into lower dimensions.
* The decoder- This network reconstructs the original data from the lower dimension representation.
The lower dimension (i.e, output of encoder network) representation is usually known as latent space representation.

The one thing which we must remember about autoencoders is that they are only able to compress the data that is similar to what they have been trained on. They are also lossy in nature which means that the output will be degraded with respect to the original input.

They are trained similarly to  via backpropagation.

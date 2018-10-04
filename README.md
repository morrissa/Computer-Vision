# Generated numerical images using GAN Computer-Vision model and MNIST data
![MNIST Generated images - computer learning how to be a trickster and draw](https://github.com/morrissa/MNIST-GAN-Generating-images-tensorflow/blob/master/GAN_MNIST.JPG)

##### In this model I aim to build a generative adversarial network to generate numerical images from the MNIST dataset comprising of the number 1 - 9

##### The generative adversarial model will be made up of two networks in one overall model which is a generator and a discriminator network/

##### a generator which will generate a fake image in order to trick the discriminator like a person making counterfeit money - trying to look as close as possible to the real image from the dataset.

##### a discriminator which will check if the image sent by the generator is real or fake, as being trained on the images within the real dataset, the output being a sigmoid of 1 or 0 - real or fake.

##### the model itself uses a leaky ReLU activation, allowing for the gradients to flow backwards, this leaky ReLU doesn't come natural to Tensorflow so it is made using using a max alpha function written as f(x) = max(a*x,x)

##### Combined with the leaky ReLU allowing for backflow in gradient and negative values, a Tanh output is used to allow the rescaling of the generated images to be between -1 and 1 instead of 0 and 1

##### as with all my models this is only a first iteration, and my plans are to continue to tinker with the model parameters and also architecture, maybe using more of a dual convolutional approach instead of just dense layers stacked.

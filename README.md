# tensorflow-dcgan-implementation
## Generative Adversarial Networks 
Generative Adversarial Networks (GANs) are types of neural network architectures capable of generating new data that conforms to learned patterns. GANs can be used to generate images of human faces or other objects, to carry out text-to-image translation, to convert one type of image to another, and to enhance the resolution of images (super resolution) among other applications. In GANs, there is a generator and a discriminator. The Generator generates fake samples of data(be it an image, audio, etc.) and tries to fool the Discriminator. The Discriminator, on the other hand, tries to distinguish between the real and fake samples. The Generator and the Discriminator are both Neural Networks and they both run in competition with each other in the training phase. The steps are repeated several times and in this, the Generator and Discriminator get better and better in their respective jobs after each repetition.

![image](https://user-images.githubusercontent.com/96515691/169303254-8364394f-7500-4f42-a637-3ada1bc9f1ff.png)

The resultant losses that arise are generator loss and discriminator loss. 

## Dataset

In the notebook, I have taken a dataset of vehicles, which is divided into subfolders of each class containing images of that particular class.

![Sample images](https://user-images.githubusercontent.com/96515691/169303965-befb7d3e-3264-4381-9355-53857ff395e4.png)

Before some preprocessing , the folders were merged into one so that the filepaths can be obtained easily. 

## Preprocessing

The DCGAN used in the notebook works for (28,28,1) shape images, hence it was necessary to resize the images. Also, the images were rescaled to suite tanh transfer function.

## Generator random noise

![image](https://user-images.githubusercontent.com/96515691/169305393-db7121dd-5d6b-43b6-9eaa-348d52dca8a3.png)

After training the model, the image after all the epochs comes out to be :

![image](https://user-images.githubusercontent.com/96515691/169306481-b926c84e-f6e9-4249-8f3e-445045581935.png)


Since this notebook was just made to implement the DCGAN , we can just ignore how badly I failed at training the network :_)


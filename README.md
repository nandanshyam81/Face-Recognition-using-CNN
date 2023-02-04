
**Face-Recognition-using-CNN**
Keras ImageDataGenerator is used for getting the input of the original data and further, it makes the transformation of this data on a random basis and gives the output resultant containing only the data that is newly transformed. It does not add the data. Keras image data generator class is also used to carry out data augmentation where we aim to gain the overall increment in the generalization of the model. Operations such as rotations, translations, shearin, scale changes, and horizontal flips are carried out randomly in data augmentation using an image data generator.So, made a model using CNN with the help of tensorflow and keras.Model will be trained on certain amount of data and then will be tested.

> The images have been loaded in batches , it is done so because if we load all images at a time, the training speed of model will become very less as we are using a lot of memory in CPU which becomes very inefficient.

> Images belonging to five famous personalities have been downloaded from Google using the batch downloader extension and were stored.Training and the test set were downloaded seperately. On an average for each class there were 90 images.
> 
> CNN generally requires high training data for its accuracy to be more.

![image](https://user-images.githubusercontent.com/109072424/216766083-39e4ee55-e802-442d-a232-d6ab6a4265ab.png)


> The convolutional layers are the initial layers to pull out features from the image.It maintains the relationship between pixels by learning features using a small input data sequence.It is a mathematical term that takes two inputs, an image matrix and a kernel or filter.Kernel is a filter that is used to extractt the features from the images.

> ReLU is used in the CNN model over the other activation functions because it improves the neural networks by speeding up training.Also, the computation step of a ReLU is easy as all negative elements are set to 0.0 and no exponentials,no  multiplication or division operations are involved.

> The pooling layer is another building block of a CNN and plays a vital role in pre-processing an image. In the pre-process,the image size shrinks by redcuing the size of the image.When the picture is shrunk, the pixel density is also reduced, the downscaled image is obtained from the previous layers.

> The final layer of the CNN model was the output layer where Softmax activation function was used. It was used over the other famous functions like Sigmoid function because Sigmoid function is more useful when we are doing only binary classification. As more than two classes were involved softmax function was used, which gives output as a probability value i.e. between 0 and 1. The highest value indicates the output would be from the particular neuron through which we can tell which class it belongs.



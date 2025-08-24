Transformers>> Deep Learning >> Software
### For what all algorithms feature Scaling is required?
ANN, Linear Regex, Logistic Regex, KNN,  KMeans
NOT- Random Forest, Decision Trees, xgBoost, AdaBoost
1. Any distance based algo 
2. Wherever Gradient Descent or Optimisers are involved how convergence will happen will be quicker

### Difference between fit_transform() and transform()
Avoid dataLeakage!
### Tensorflow is created by Google DeepMind Team
Pytorch by Fb  both re same
 Before tensor 2.0 was sepearte Keras(wrapper) uses tensorflow APIS only.
 After 2.0 both got integrated Tensorflow+Keras

 ### Sequential Model VS Dense Layer 
"Sequential" refers to a type of model, while "Dense" refers to a specific type of layer within that model.
Sequential Model:The Sequential model in Keras represents a linear stack of layers, where data flows sequentially from one layer to the next. It is the simplest and most common type of model for building feedforward neural networks. 
A ### Dense layer, also known as a fully connected layer, is a fundamental type of layer in neural networks. In a dense layer, every neuron in the layer is connected to every neuron in the preceding layer. 
  ### Operation:
        It performs a matrix-vector multiplication, where the input is multiplied by a weight matrix (trainable parameters) and a bias vector is added. An activation function is then typically applied to the result.
### Purpose:
Dense layers are used to learn complex patterns and relationships within the data, often serving as the final classification layer or for projecting feature representations into a different dimension.
### The Dense layer applies the following mathematical operation: output=activation(dot(input,kernel)+bias)
where:
activation: An element-wise activation function (if specified).
dot(input, kernel): A matrix multiplication between the input data and the weight matrix (kernel).
bias: A bias vector added to the computation (if use_bias=True).
This means every neuron receives a weighted sum of all the inputs, applies an activation function, and then passes the result to the next layer.
### DropuOut:- 
### Early stopping: When accuracy of model is not at all ncreasing, stop the training no what how many epoch is left.

### Activation layer 


### CNN is an Artificial Neural Network (ANN) widely used for analysing images can be used for other data anaysis and classification problems.
CNN is an ANN which has some type of specialization for being able to find or pick out patterns,which makes them suitable for image analysis. 
- CNN has hidden layers called as convolutional layer.
- ### convolutional layers do?
    they receives input and tranform the input in some way and outputs that input to next layers, with convolutional layer this transformation is a convolutional operation.
    - are able to detect patterns in the images.
       - with each convolutional layer we need to specify the number of filters it has, it is a small  matrix where we define number of rows and columns, values in the matrix has random numbers
Image is either B&W or RGB
in B&W images there is a single channel onl with grids each pixel is ranging between 0-255 0-black 255-white
and in RGB there are 3 channels R, G, B

example:-
we have a image which will be passed through a filte and we will get a output 
1stly we wil try to make the pixel value between 0&1 if they are not already by % by 255 } ### Process is Min-Max Scalling!

# deeplearning-project

company name: CodeTech IT solutions

Name : Mahendra B

Domain : Data Science

Duration : 4 Weeks

Intern ID : CTIS6932

Mentor : Neela Santosh

Descripition of the task :

The objective of this task is to build and train a basic neural network model using the PyTorch library to classify handwritten digits from the MNIST dataset. This task introduces fundamental concepts of deep learning, including dataset handling, model creation, training, and performance visualization.

The process begins with importing the required libraries such as PyTorch, Torchvision, and Matplotlib. Torchvision provides access to popular datasets and image transformations, making it easier to work with image data. In this task, the MNIST dataset is used, which contains grayscale images of handwritten digits ranging from 0 to 9. Each image is of size 28×28 pixels.

Before feeding the data into the model, a transformation is applied using transforms.ToTensor(). This converts the images into tensors and scales pixel values to a range between 0 and 1. The dataset is then loaded using torchvision.datasets.MNIST, where the training portion of the dataset is downloaded and stored locally. To efficiently process the data during training, a DataLoader is used, which divides the dataset into batches and shuffles the data to improve learning.

The next step is defining the neural network model. In this task, a simple feedforward neural network is implemented using nn.Sequential. The model consists of a flatten layer that converts the 2D image into a 1D vector, followed by a fully connected (linear) layer with 128 neurons and a ReLU activation function. The final layer outputs 10 values, corresponding to the 10 digit classes (0–9).

To train the model, a loss function and an optimizer are defined. The CrossEntropyLoss is used because it is suitable for multi-class classification problems. The Adam optimizer is chosen for updating the model parameters, as it is efficient and widely used in deep learning tasks.

The training process is carried out over multiple epochs. In each epoch, the model processes all batches of training data. For each batch, the gradients are reset, predictions are made, the loss is calculated, and backpropagation is performed to update the model weights. The total loss for each epoch is accumulated and stored for later analysis. Printing the loss after each epoch helps monitor how well the model is learning.

After completing the training process, the task includes visualizing the training performance. A graph is plotted using Matplotlib, showing the loss values across epochs. This visualization helps in understanding whether the model is improving over time. Ideally, the loss should decrease with each epoch, indicating that the model is learning effectively.

output of the task :


In conclusion, this task demonstrates the complete workflow of training a simple neural network for image classification using PyTorch. It covers essential steps such as data preprocessing, model design, training, and evaluation through visualization. This serves as a foundation for more advanced deep learning applications in computer vision.

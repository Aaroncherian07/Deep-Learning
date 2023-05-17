##Deep Learning##

Background
This assignment deals with the implementation from scratch of relatively simple deep learning models and techniques for transfer learning of object detection models for computer vision applications. You should be able to complete the whole assignment without access to large computation cluster and relying only on your laptops or online training tools (e.g. Google Colab). If you have issues, you can setup a remote access to one of our Cranfield machines in the PC labs – contact SASAAI about this.

Brief
Task 1 – Image classification on the MNIST handwritten digits recognition dataset
The MNIST handwritten digits dataset was mentioned and discussed during the lectures several times. 
Task 1a. You are asked to train 2 different models:
1.  Model A) Recurring only the fully connected (i.e. dense) layers.
2.  Model B) A convolutional neural network for handwritten recognition. Appropriately discuss the architecture and the hyperparameters chosen.

Task 1b. Please demonstrate that you monitored the training of the neural network by monitoring appropriately the loss-function, the accuracy, and confusion matrix. Demonstrate the performance of the models relying on appropriate graphs and discuss the differences between FC and CNN classifier.

Task 1c. 1). Apply a pre-trained network (Alexnet, VGG, ResNet, etc.) to the network and select one layer to visualize the activation of the learned feature map. 2) Design a state-of-the-art classifier based on the MNIST dataset that will be able to beat LeNet 1998 model (98.7% accuracy on the test set). Demonstrate that your model does not overfit the data.

Task 2 – UAV Object Detection using transfer learning
You are provided a small dataset with images of UAV. The labels of the dataset contain the parameters for a bounding box regression of the dataset. You can download the full dataset from CANVAS. As you will notice, this is a relatively small dataset. This means that you are not going to be able to train an object detector from scratch on such a small dataset.Information categorisation:

Task 2a.
Start by selecting 12 samples for both training and testing data and plot in 3x4 subplot format indicating:
1.        Plot the labels and verify the label format: [x y width height].
2.        Pre-process the data set and split the data set in training/validation/testing set, explain your data split strategy.

Task 2b. 
Your aim is to train an object detector which achieves a good performance on the dataset and detects the position of UAVs in the picture. You need to apply and compare two different object detection networks, and one of it should be YOLO networks (no requirement to the specific version). You don’t have constrains about computational time (for inference) so you can opt also for two- stage detectors.
Students are supposed to understand how to fine-tune a pre-trained deep neural network to detect UAVs. Solve the issues in the transfer progress, such as pre-process the data set and adjust the layer architecture. The choice of model is up to the student (there isn’t necessarily a single correct answer).
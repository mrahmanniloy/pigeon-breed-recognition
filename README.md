The Summary for the Source Code of the Pigeon Breed Recognition using Convolutional
Neural Network Project
1. Importing dataset: In this section, I imported the dataset of pigeon breed images which was
stored in google drive.
2. Importing packages: In this section, I imported all the Python and Deep Learning packages into
the coding environment.
3. Exploring the data: Here, I checked randomly selected ten (10) images from every one of the
training, validation and test folders of the dataset.
4. Data preprocessing: In this section, I created one image data generator variable from the
dataset for each of the train, validation and test purposes of the models. Only the training data
generator was created with additional increase of the training data using image augmentation.
5. Building model
5.1 Main model: Here, I created a baseline model with four convolution layers and two dense
layers.
5.2 Modified model: Here, I created another model which has four convolution layers but with an
increased number of neurons and four dense layers.
5.3 Model compiling: In this section, I compiled the selected model with adam optimizer,
learning rate of 0.001, categorical cross entropy to calculate loss and accuracy as the metric.
5.4 Early stopping: Here, the EarlyStopping function from the keras callbacks module was used
to stop the training of the model when the value of the validation loss does not decrease
anymore.
5.5 Model checkpoint: Here, the best classifier model was saved in the hierarchical data format
(model.h5) where the threshold value was the highest validation accuracy.
6. Tensorboard: The tensorboard library was loaded here in order to visualize and monitor the
whole training and validation process.
7. Training: In this section, the model was trained for 200 epochs with the additional callback
functions.
8. Evaluating accuracy and loss for the model
8.1 Accuracy visualization: Here, the accuracy of the trained model at each epoch was
visualized using a generated graph.
8.2 Loss visualization: Here, the loss of the trained model was visualized.
8.3 Confusion matrix and classification report visualization: The confusion matrix and the
classification report was generated here.


# Plant leaf classification
**Assignment 1** of  the course *Artificial Neural Networks and Deep Learning* at *Politecnico di Milano*: Deep Learning models to classify images of leafs, which are divided into categories according to the species of the plant to which they belong.

We were provided with the training dataset, while models were evaluated on a hidden test dataset.

Project realized with *Keras* module in *Python*

## Dataset
Details about the dataset and some exploratory data analysis are reported in the provided Python notebook [dataLoading](https://github.com/denaldo98/leaf_plant_classification/blob/main/dataLoading.ipynb).

As can be seen in the [notebook](https://github.com/denaldo98/leaf_plant_classification/blob/main/dataLoading.ipynb), the provided dataset is highly unbalanced. 
To deal with that we adopted two strategies to split the provided dataset into training and validation:
 1. Splitting the dataset uniformly and applying corrective class weights
 2.  Splitting with oversampling

Moreover, we applied data augmentation by using the [ImageDataGenerator](https://www.tensorflow.org/api_docs/python/tf/keras/preprocessing/image/ImageDataGenerator) class of *Keras*.

The notebok [notebookFinal](https://github.com/denaldo98/leaf_plant_classification/blob/main/notebookFinal.ipynb)  contains the best models developed to solve the task. 
In order:

 1. CNN model (without transfer learning)
 2. Transfer Learning model (Xception)
 3. Fine Tuning model (Xception)

Development steps, training plots and obtained performances are reported in the [report file](https://github.com/denaldo98/leaf_plant_classification/blob/main/Challenge1_AN2DL.pdf).

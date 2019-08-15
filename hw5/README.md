# Week 5 Mini-Project
## Self Supervised Learning for Image Classification

In this Mini-Project you will be implementing a paper that uses geometric transformations to extract features of an image without requiring these images to be labeled. This project will be for the most part from scratch; however, feel free to use the documentation below or reach out to club members to guide you. You have two weeks to complete the project and there will be regular checkpoints as outlined below. Good luck!

### Project Objectives
In this project you will learn the following valuable skills:
1. Using tensorflow data API to load and preprocess data
2. Utilizing CPUs and GPUs for async processing
3. Using tensorboard to visualize training curves
4. Training a model from scratch and frequently checkpointing models
5. Visualizing the features of your network

### Project Checkpoints
1. Complete code logic. Set up AWS instance.
2. Complete training and show results. Date: TBD
3. Completed project with feature visualization and results is due on Monday at 8pm SHARP. NO EXCEPTIONS ON THIS DEADLINE.

### Setting up your environment
`pip3 install vitrualenv` (if not already installed)
`virtualenv venv`
`source venv/bin/activate`
`pip3 install -r requirements.txt`


To deactivate the environment you are in run:
`source deactivate`

### Downloading the CIFAR-10 dataset
#### You can read more about the CIFAR-10 dataset here: https://www.kaggle.com/c/cifar-10
1. Go to this link https://www.cs.toronto.edu/~kriz/cifar.html
2. Right click on "CIFAR-10 python version" and click "Copy Link Address"
3. Go to your CLI and go into the `data` directory.
4. Run this cURL command to start downloading the dataset: `curl -O <URL of the link that you copied>`
5. To extract the data from the .tar file run: `tar -xzvf <name of file>` (type `man tar` in your CLI to see the different options for running the tar command). 
**NOTE**: Each file in the directory contains a batch of images in CIFAR-10 that have been serialized using python's pickle module. You will have to first unpickle the data before loading it into your model.

### Using Tensorflow dataloaders
Resource: https://www.tensorflow.org/guide/datasets

### Saving and Restoring Models
Here is an excellent guide on how to save and restore models in tensorflow
https://cv-tricks.com/tensorflow-tutorial/save-restore-tensorflow-models-quick-complete-tutorial/
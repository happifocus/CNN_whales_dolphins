#### CNN_whales_dolphins
A setup for a CNN to classify between images of back fins from whales and dolphins. 

# CNN using TensorFlow + Keras to classify images of whales and dolphins

Whales and dolphins are endangered species and are important to the 
balance of the marine ecosystem. To protect these animals, it is important 
to monitor their appearance and population size. To monitor and identify 
different species, or even individuals, it became common to take 
photographs of backs and back fins.

While attending the WBS Data Science Bootcamp, I wanted to learn more 
about image classification by building a Convolutional Neural Network 
(CNN). The motivation of this project is to find a quick method to sort 
taken photographs of dolphins and whales for further analysis and 
statistics. 

The dataset was taken from a Kaggle competition. The available training 
data contained a mix of dolphin and whale images, which got split into 
separate folders by using the information of a given CSV-file to create 
two classes of images: dolphins and whales. 

## Sources and Credits

To retrieve more background information and to access data used in this 
project, follow the source link of the Kaggle competition: 

[Kaggle: Happy whale and 
dolphin](https://www.kaggle.com/competitions/happy-whale-and-dolphin/overview)

The actual CNN was built by following the inspirational tutorial of 
Nicholas Renotte:

[Build a Deep CNN Image Classifier with ANY 
Images](https://www.youtube.com/watch?v=jztwpsIzEGc)

## Project description

- This application is based on Jupyter Notebooks, running Python code.
- Main data from Kaggle was downloaded and locally stored into a main 
project folder.
- Basically, there are two different notebook to 
	1.) split main data into two classes, and 
	2.) to run the actual CNN (based on TensorFlow and Keras) using a basic setup.
- The CNN was set to perform binary image classification, to distinguish between back fins from dolphins and whales. 
- For performance evaluation, a scoring of accuracy, loss, validation accuracy, 
validation loss, precision and recall is included. 
- Performance values are separately stored in CSV-files and plotted as graphs.

## Faced challenges

- While training the network, it wasn’t possible to reach an overall accuracy higher 
than 90 %. Trying to add regularization methods did not remarkably improve the 
performance and accuracy score.
- Also, using different image input sizes didn’t improve the training. Trying to work 
with larger image input sizes (i.e. 256x256) meant to remove a part of training data, 
and therefore reducing training capabilities. 
- In general, training images highly varied in shape and size, ranging between 2 KB and 
5.8 MB. 
- Another difficulty might be that some characteristic back fins of dolphins and whales 
were taken from different angles, and thus appearing similar to each other, introducing 
uncertainties to properly get differentiated by the CNN. 

## Project requirements

Working environment: 
- Anaconda distribution 
- Python
- Jupyter Notebook

Required packages to install within used Anaconda environment: 
- jupyter
- tensorflow 
- tensorflow-GPU
- os
- opencv (cv2)
- numpy
- matplotlib

Using Anaconda is the easiest way to perform Python and R. Having Anaconda installed, 
there is no need to install Python separately, because it is already part of the 
Anaconda distribution.

### 1. Install Anaconda

- to work with Anacondam follow the [general Anaconda 
documemntation](https://docs.anaconda.com/anaconda/install/index.html)
- install Anaconda on [Windows](https://docs.anaconda.com/anaconda/install/windows/)
- install Anaconda on [macOS](https://docs.anaconda.com/anaconda/install/mac-os/)
- install Anaconda on [Linux](https://docs.anaconda.com/anaconda/install/linux/)
- alternatively, Anaconda offers [installation packages](https://www.anaconda.com) for 
Windows, macOS and Linux  

### 2. Run/open Anaconda Navigator

### 3. Anaconda environments

Navigate to the Environments section of the Anaconda Navigator. Here, all available 
working environments are listed. When freshly installed, there is only one environment 
listed, which is mainly named as: base (root). 
Within this section, additional environments can be created, holding different setups of 
installed packages and dependencies. To add a new environment, click on the create/+ 
button at the bottom and provide a simple and descriptive name.

### 4. Jupyter Notebook on Anaconda

By default, the Jupyter Notebook application should be available. After selecting a 
desired environment, go to the Home section of the Anaconda Navigator to see all 
available applications listed. If Jupyter Notebook can’t be found (especially after 
creating a new environment), it needs to be added to the active working environment.  

### 5. Add packages (libraries) to Anaconda environment

To add required packages, such as jupyter, tensorflow, tensorflow-GPU, os, opencv (cv2), 
numpy, matplotlib, first choose the dedicated environment and select for not installed 
in the pull-down menu shown at the top of the Navigator. Use the search bar at the top 
right to enter the name of specific packages to be installed: i.e. enter jupyter to find 
available packages, select by clicking the checkbox (always choose the main package 
first), and press Apply to fully install. Repeat these steps for all listed dependencies 
like tensorflow, tensorflow-gpu, os, opencv, numpy and matplotlib. 

## Work on the project

### 1. Set main directory

Set a main working directory by creating a main project folder named **Project_whales_dolphines** or similar.

### 2. Download data

Download related data from the [Kaggle competition 
site](https://www.kaggle.com/competitions/happy-whale-and-dolphin/data). 
To save data, almost 63 GB of storage space is required. Unzip downloaded data and add 
them to the main project folder **Project_whales_dolphins** .

### 3. Download notebooks

Download the two notebooks from the GitHub repo and add them to the main project 
folder **Project_whales_dolphins** .

### 4. Summary of main project folder

The main project folder **Project_whales_dolphins** should contain: 
- two notebooks
- the **train.csv** file
- the **train_images** folder

### 5. First notebook: split data

The first notebook is about data preparation. Follow the instructions to separate images 
of whales and dolphins from the **train_images** folder into two new folders.

### 6. Adjust data path and create subfolder

Within the main project folder **Project_whales_dolphins** , create a main data 
folder **DATA** containing the two separate folder for images of whales and 
dolphins as subfolder (Project_whales_dolphins -> DATA -> whale, dolphin).  

### 7. Second notebook: train CNN

Continue to work with the second notebook: load data from the main data folder **DATA** and train the network. The two subfolder **whale** and **dolphin** are 
automatically recognized as classes to be trained on. 

### 8. Second notebook: test the model

For testing, copy image data from the **testing_images** folder into the 
main project folder **Project_whales_dolphins** (just beside the second notebook) 
and run the model prediction.

### 9. Support and Authorship

19.01.2023, contact on [LinkedIn](https://www.linkedin.com/in/danielavorkel/)


# ACSE9-FINAL-project
User Guide
============================

### Compilation/Installation Guide

This software is fully developed under Google Colab Platform since the project relys heavily on machine learning strategies. For a quick intro to Google Colab, click this link https://colab.research.google.com/notebooks/intro.ipynb. 

To import the code along with documentions, project plan and the final report, go into the terminal and enter:
```
git clone https://github.com/acse-2019/irp-acse-ll2819.git
```
### User instructions

The training set, encoded data from images and weights of models are extremely large files and folders that cannot be pushed to the Github repository directly. If user wants to re-run the programs on their own, please go to the link https://drive.google.com/drive/folders/1gadn2CHJxWjQeo9gqA5gq-oGPszRAOxP?usp=sharing to download the folder **./data** and **./models**. And make sure put these folders in the following directory structure:   
```
./Code
--/acse9
----/code            
------------/Autoencoders_RBMs_training     # training models and extracted the latent representations of images
------------/Data_Preprocessing             # functions of data preprocessing
------------/Semantic_Segmentation_Training_and_Visualization   # training semantic segmentation models and visualize the results
------------/Unsupervised_Classification_and_Visualization      # classify the features and visualize
----/data
------------/encoded_data                  # the latent representations of images with edge detection technique: outputs of Autoencoders_RBMs_training
------------/encoded_data_no_edge          # the latent representations of images without edge detection technique: outputs of Autoencoders_RBMs_training
------------/Labelled_Image                # the dataset used for training semantic segmentation models
----/models
------------/autoencoders                  # saved autoencoder and RBMs models trained with edges
------------/autoencoders_no_edge          # saved autoencoder and RBMs models trained with original images
------------/segmentation                  # saved segmentation models trained with edges
------------/segmentation_original_image   # saved segmentation models trained with original images
``` 
Then upload the **acse9** folder to google drive, and run the files in **code** directory. Make sure the path is '/content/gdrive/My Drive/acse9'.

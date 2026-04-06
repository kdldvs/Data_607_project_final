# Data 607 Project – Wildlife Image Classification

## Overview
This project uses camera trap images from Alberta (Friends of elk island 2020. [1] WildTrax dataset) to build image classification models (CNN / Vision Transformer) to identify animal species.


To run this repo first download the FEIS_Friends_of_Elk_Island_2020_image_report.csv and FEID_Friends_of_Elk_Island_2020_tag_report.csv from the Friends of elk island wildtrax repository [1] and insert them into the main folder of this repo.


Then use the Data_607_Project_Dataset_Ingestion.ipynb to ingest data from wildtrax changing the absolute path in the notebook to one of your choice to save the images. This downloads the full-sized images and creates the dataset_labels.csv for use in running the models.

This can be followed by running Resize_images.ipynb to get the images resized into a 256x256 format for the CNN.

The EDA, VIT, and CNN notebooks can then be run to use the images for exploratory data analysis, training the pretrained vision transformer, or training the convolutional neural network respectively.

The requirements.txt includes the libraries needed to run using CUDA 12.X for pytorch, however, some environment management may be needed for the EDA or if a different version of pytorch is needed.

[1] WildTrax, Friends of elk island 2020, Accessed: 2026-03-18, n.d. [Online]. Available: https://portal.wildtrax.ca/cam/354
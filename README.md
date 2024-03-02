# **Intestinal Parasitic Egg Classification in Microscopic Images using CNNs**
MSDS692: Data Science Practicum I Project
Author: Lonny Cox-Lauf

## Purpose

![alt text](parasite_eggs_11.png "Sample Microscopic Image for each of the 11 Parasitic Egg Classifications")

TO DO

## Tools

TO DO

## Dataset Description

TO DO

## Image Data Cleaning

The images had to be:

* Unzipped into Google drive
* Cropped using their corresponding bounding boxes (found in the labels.json file that accompanied the image dataset)
* Image files were broken out into subdirectories for each class (label) and training, validation, test splits as well

## Evaluation of Best Model Performance

EfficientNetB0 CNN architecture as the base for the model achieved a F1-score of 0.84714 when making class predictions on the test set.

![alt text](ConfMat_EfficientNetB0.png "Confusion Matrix")

## Conclusion

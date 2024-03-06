# **Intestinal Parasitic Egg Classification in Microscopic Images using CNNs**
MSDS692: Data Science Practicum I Project
Author: Lonny Cox-Lauf

## Purpose

Intestinal Parasitic Infections (IPIs) are one of the most common causes of illness in the world, and they can cause harsh symptoms and even death in some cases. These symptoms can include (but are not limited to): nausea, nutritional deficiency, abdominal pain, and more. IPIs typically manifest themselves in developing locations, such as sub-Saharan Africa, the Caribbean, and Asia. 

## How to Run the Project in Google Colab

TO DO

## Dataset Description

![alt text](parasite_eggs_11.png "Sample Microscopic Image for each of the 11 Parasitic Egg Classifications")

The dataset contains 11 classes of parasitic eggs, with each class containing 1,000 images. This gives a total of 11,000 images. The images were taken as microscopic images from human faecal samples, all of which contain intestinal parasitic infectious (IPI) eggs in view. The quality of image varies greatly, as some images are more blurry than others, and some are more zoomed in on the egg while others are zoomed out. This all adds to the complexity of this image classifier project.

## Image Data Cleaning

The images had to be:

* Unzipped into Google drive
* Cropped using their corresponding bounding boxes (found in the labels.json file that accompanied the image dataset)
* Image files were broken out into subdirectories for each class (label) and training, validation, test splits

## Evaluation of Best Model Performance

EfficientNetB0 CNN architecture as the base for the model achieved a F1-score of 0.84714 when making class predictions on the test set. This strong F1-score indicates that *both* the precision *and* recall were favorable, as F1-score is the harmonic mean of precision and recall metrics. In other words, if either precision or recall was relatively low, the F1-score would be brought down much more than if the calculation was simply the statistical (standard) mean of precision and recall.

See below for a confusion matrix representing the correct prediction counts (on the main diagonal) and incorrect prediction counts (off the main diagonal):

![alt text](ConfMat_EfficientNetB0.png "Confusion Matrix")

## Conclusion

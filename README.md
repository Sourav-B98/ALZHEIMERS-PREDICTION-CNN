# MRI image analysis for Alzheimer's disease prediction

This repository contains all code snippets and powerpoint presentation for a Machine Learning Course project focused on Alzheimer diagnosis using Deep Learning and MRI images. The files and folder structure are organized in the following way:

* `presentation.pdf` is the presentation that was used for formal presentation of the project.Key points are highlighted there.

*  the `CODE` folder contains the jupyter notebooks used in Google Colaboratory for the development of the deep learning models. It contains the following notebooks:

* 'EDA' . Exploratory analysis of the dataset, some insights explained in the presentation.pdf.

* `Preprocess`. Several experiments and organization of the MRI images. Image registration and skull-stripping is performed in this notebook, as well as other experiments useful for familarizing with the image format (`.nii`).

* `TFrecords`. Using the preprocessed images, several TFRecords files are created in this notebook. This file format is much faster to read than native Python generators, and does not consume as much RAM as loading all images in memory.

* `tuning InceptionV3`. First model built. Fine-tuning an InceptionV3 network trained with ImageNet for classifiying between healthy, demented and MCI patients.

* `ResNet3D`. Second model built. Training a 3-dimensional residual network for classifiying between healthy, demented and MCI patients.



The data used for the development of this project could not be placed on this repository, since the MRI images are private and were obtained from the Alzheimer's Disease Neuroimaging Initiative (ADNI) database.


CT Scan Image Classification Project
Project Overview
This project aims to develop a deep learning model for the classification of CT (Computed Tomography) scan images. The model will be trained to identify specific patterns or abnormalities within CT scans, which can have applications in medical diagnosis and healthcare.

Prerequisites
List the software, libraries, or hardware requirements necessary to run your project. For example:

Python 3.6+
keras
matplotlib
NumPy
Pandas

Data Augmentation

* `rotation_range` is a value in degrees (0-180), a range within which to randomly rotate pictures
* `width_shift` and `height_shift` are ranges (as a fraction of total width or height) within which to randomly translate pictures vertically or horizontally
* `rescale` is a value by which we will multiply the data before any other processing. Our original images consist in RGB coefficients in the 0-255, but such values would be too high for our models to process (given a typical learning rate), so we target values between 0 and 1 instead by scaling with a 1/255. factor.
* `shear_range` is for randomly applying shearing transformations
* `zoom_range` is for randomly zooming inside pictures
* `horizontal_flip` is for randomly flipping half of the images horizontally --relevant when there are no assumptions of horizontal assymetry (e.g. real-world pictures).



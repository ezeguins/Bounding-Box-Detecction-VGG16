# BOUNDING BOX DETECTION VGG16
Python Google Colaboratory Notebooks - Contacts Images files Bounding Box Detection. 
The original data set was obtained from corporate documents and is the property of MERCADOLIBRE and is not shared due to confidentiality reasons.


## Files:
### CV2_filters_ts.ipynb
PREPROCESSING DATASET: OpenCV FILTERS TO IMPROVE FILES
- convert to grayscale
- noise removal
- thresolding
- dilation
- erosion
- canny edge detection
- skew correction

### augmentation_ts.ipynb
DATA AUGMENTATION FOR BOUNDING BOX DETECTION DATASET
- Load dataset file from gdrive.
- Divide in three equal parts and rotate images and boundig boxes 90, 180 and 270 degrees.
- Save to gdrive rotated data and annotations with their new filesnames.

### dataset_generator_ts.ipynb
GENERATE .NPZ DATASET FILE FROM TWO DIFFERENT CVS ANNOTATIONS FILES

First dataset genertion and second dataset generation attached to the first one.
Record file to current gdrive 

### labeling_visualization_ts.ipynb
THIS NOTEBOOK IS USEFUL TO VISUALIZE THE BOUNDING BOX DATASET AND THE ANNOTATIONS (LABELING)  

### model_training_ts.ipynb
THE NOTEBOOKS PERFORMS THE FOLLOWING:

- Load the dataset generated at "dataset_generator_ts.ipynb" file
- Initialize model parameters
- partition the data into training and testing splits using 90% of the data for training and the remaining 10% for testing
- Load the VGG16 network with "imagenet" weights, ensuring the head FC layers are left off
- Construct the model we will fine-tune for bounding box regression
- Initialize and train de model
- Plot results and model training history

### predict_txt_ts.ipynb
BOUNDING BOX MODEL PREDICTION FROM .TXT FILE CONTAINING TEST IMAGES FILENAMES GENERATED IN THE "model_training_ts.ipynb" FILE

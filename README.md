# VGG16
Python Google Colaboratory Notebooks - Contacts Images files Bounding Box Detection. 

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

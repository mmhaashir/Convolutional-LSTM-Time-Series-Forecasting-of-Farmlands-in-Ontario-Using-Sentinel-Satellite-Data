# Convolutional LSTM Time Series Forecasting of Farmlands in Ontario Using Sentinel Satellite Data

## Introduction <a name="intro"></a>
Welcome to the Time-Series Forecasting of Farmlands in Ontario, Canada project! This repository provides an in-depth guide and codebase for leveraging Convolutional Long Short-Term Memory (Conv-LSTM) networks to forecast farmland dynamics in the beautiful province of Ontario, Canada, utilizing data from the Sentinel-2 Earth-observing satellite mission.

![dav_image](https://vitalflux.com/wp-content/uploads/2022/04/different-types-of-time-series-forecasting.png)

## Table of Contents

- [**Introduction**](#intro)
- [**Dependencies**](#dep)
- [**Dataset**](#data)
- [**Installation**](#install)
- [**Results**](#results)
- [**Contribution**](#contr)
- [**Conclusion**](#conc)

## Dependencies <a name="dep"></a>

To run this code, you will need the following Python libraries:

  - Sentinelhub
  - Numpy
  - Pandas
  - Matplotlib
  - Scipy
  - Tifffile
  - Patchify
  - CV2
  - SkImage
  - Tensorflow

## Dataset <a name="data"></a>

  1. It uses data from sentinelhub, we get the satellite images from there.
     
  2. You can get the ground data [here](https://www.kaggle.com/datasets/mmhashir/ground-data)
     
  3. You can get the masked data [here](https://www.kaggle.com/datasets/mmhashir/masked-data)

## Installation <a name="install"></a>

1. Clone the repository:
   `git clone https://github.com/mmhaashir/Convolutional-LSTM-Time-Series-Forecasting-of-Farmlands-in-Ontario-Using-Sentinel-Satellite-Data.git`
   
2. Install the required dependencies:
   `pip install sentinelhub numpy pandas matplotlib scipy tifffile patchify cv2 skimage tensorflow`

## Results <a name="results"></a>

After runnning the notebook, you'll see the outputs in the form of folders of images. `stacked_images` folder containes stack of the images. Each year contains 9 images, all of the 9 are stacked into one .tiff image. So you get 4 .tiff images.

`stacked_images_updated` contains the stacked images but the singleton dimension has been removed so that it can be processed.

`masked` folder contains the stacked images but masked with the ground truth and the masking images.

`predicted_sequence` contains the output of the model, i.e. the stacked image for the next year.

## Contributing <a  name="contr"></a>

Contributions to this project are welcome. If you have suggestions or improvements, please open an issue or submit a pull request.

## Conclusion <a name="conc"></a>

This project showcases the use Convolutional LSTM for time series forecasting of stacked images.

Feel free to experiment with different images, and datasets to gain deep understanding.

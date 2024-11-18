# Multiclass-Classification-with Satellite-Data

- The dataset comes from the <a  href='https://archive.ics.uci.edu/ml/datasets/Statlog+%28Landsat+Satellite%29'>UCI machine learning website</a>. It consists of the multi-spectral values of pixels in 3x3 neighbourhoods in a satellite image, and the classification associated with the central pixel in each neighbourhood. 
- The aim is to predict this classification, given the multi-spectral values. In the sample database, the class of a pixel is coded as a number.

## Details
- The database is a (tiny) sub-area of a scene, consisting of 82 x 100 pixels. Each line of data corresponds to a 3x3 square neighbourhood of pixels completely contained within the 82x100 sub-area. Each line contains the pixel values in the four spectral bands (converted to ASCII) of each of the 9 pixels in the 3x3 neighbourhood and a number indicating the classification label of the central pixel. The number is a code for the following classes:

 
#### **Number Class**
1. red soil
2. cotton crop
3.  grey soil
4. damp grey soil
5.  soil with vegetation stubble
6. mixture class (all types present)
7.  very damp grey soil

## Concept
- Preprocessing data by split string and restructure into dataframe.
- Visualizing the satellite data with 4 channels (1-3rd are RGB, 4th is Near-infrared) each of 3x3 pixels
- Prepared data using Label Encoder to turns label column to numerical classes.
- Create baseline model (DummyClassifier) as an initial model utilizing simple strategies for prediction.
- Create LogisticRegression model and  RandomForestClassifier model with difference strategies
- Evaluate and compare each model with performance by confusion matrix.
- Test the best model with test set (unseen dataset).

![4channels grey ](https://github.com/user-attachments/assets/2b4afda8-ef83-473e-b6b2-588052f4f725)
![4channels ](https://github.com/user-attachments/assets/7fab925a-82dc-47d0-bac4-f92fb083597d)

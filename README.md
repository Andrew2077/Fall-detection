<!-- # Fall-detection
 Time-series analysis for fall detection

## Project Description
- This project is to detect fall from time-series data that were gathered from a wearable device containing accelerometer.
- The main goal is to design a model that can detect fall from the time-series data.


## Data
- Data was gathered from only 1 subject, and where only tested on the subject.
- data contains 3 different activities: walking, falling, and Knelling.


## Preprocessing
- Noise were removed from the data manually to ensure that the data is clean.
- labels were added to the data to indicate the activity type correclty.
- during the preproccessing phase the deravitive of the movement across all axies were taken into conceration for better results.

## Model Design
- Bi-directional LSTM to the sequence of the movement across all axies.
- MLP to classify the activity type based on the captured sequence.

## Results
- Duo to having only 1 subject, and small amount of data.
- the model was seemingly overfitting the subject.

## Quantization 
- Dynamic range quantization was used to reduce the model size.
- Conversion to tflite was done to be able to run the model on mobile devices. -->


# Fall Detection
Time-Series Analysis for Fall Detection

## Project Description
This project aims to detect falls from time-series data collected from a wearable device containing an accelerometer. The primary goal is to design a model capable of accurately detecting falls from the given time-series data.

## Data
The data was gathered from a single subject and exclusively tested on the subject. It comprises three different activities: walking, falling, and kneeling.

## Preprocessing
To ensure clean data, noise was manually removed. Labels were added to indicate the activity types correctly. Additionally, during the preprocessing phase, the derivative of the movement across all axes was considered for improved results.

## Model Design
The model design consists of a Bi-directional LSTM to analyze the movement sequence across all axes, followed by an MLP to classify the activity type based on the captured sequence.

## Results
Due to the limited data with only one subject, the model exhibited signs of overfitting to the subject.

## Quantization
Dynamic range quantization was employed to reduce the model size, and conversion to tflite format enabled the model's deployment on mobile devices.
# Movie Frame Prediction
10개의 Serial Frame을 Input으로 받아 다음 10개의 Frame을 Predict하는 Project입니다.
<img src = "https://github.com/focalpoint94/ML_MovieFramePrediction/blob/main/pics/Project.JPG?raw=true" width="100%" height="100%">


# Result
Test Data에 대한 Prediction 결과입니다.
- Test Input
<img src = "https://github.com/focalpoint94/ML_MovieFramePrediction/blob/main/pics/Input%20Example.gif?raw=true" width="50%" height="50%">

- Test Output
<img src = "https://github.com/focalpoint94/ML_MovieFramePrediction/blob/main/pics/Output%20Example.gif?raw=true" width="50%" height="50%">


# Model Description
모델은 아래와 같이 구성됩니다.
1) AutoEncoder 학습시키고, Encoder와 Decoder를 분리하여 이후 단계에 사용합니다.
2) Encoder를 통해 Input Image의 Feature를 뽑아내고, 이를 LSTM에 통과시킵니다.
3) LSTM Output을 Decoder를 통과시켜 Image를 생성합니다.
<img src = "https://github.com/focalpoint94/ML_MovieFramePrediction/blob/main/pics/AutoEncoder.JPG?raw=true" width="50%" height="50%">
<img src = "https://github.com/focalpoint94/ML_MovieFramePrediction/blob/main/pics/LSTM.JPG?raw=true" width="50%" height="50%">

## Encoder
<img src = "https://github.com/focalpoint94/ML_MovieFramePrediction/blob/main/pics/Encoder.png?raw=true" width="50%" height="50%">

## Decoder
<img src = "https://github.com/focalpoint94/ML_MovieFramePrediction/blob/main/pics/Decoder.png?raw=true" width="50%" height="50%">

## LSTM
<img src = "https://github.com/focalpoint94/ML_MovieFramePrediction/blob/main/pics/LSTM.png?raw=true" width="50%" height="50%">


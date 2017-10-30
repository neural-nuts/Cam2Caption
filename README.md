# Cam2Caption
An Android application which converts camera feed to natural language captions in real time.
The app uses a trained model generated through [image-caption-generator](https://github.com/neural-nuts/image-caption-generator).

The trained model to run this app can be obtained [here](https://drive.google.com/open?id=0ByhzM2YklhADNmk4cEN2MTA5U0E).

## Software Pre-Requisites
1. Android-Sdk
2. Android-Studio
3. Tensorflow Java Library
  - Already provided build #44 in this repository. Latest nightly builds can be obtained frome [here](https://ci.tensorflow.org/view/Nightly/job/nightly-android/)
  - *Warning*: Did not test this app with builds other that #44  

## Data Pre-Requisites
1. Trained model from [image-caption-generator](https://github.com/neural-nuts/image-caption-generator)
2. Word IDs to Word map pickle from [image-caption-generator](https://github.com/neural-nuts/image-caption-generator) currently provided in `Application/src/main/assets`


## Instructions
To build this app for your android phone-
1. Clone this repository
2. Download the trained model from [here](https://drive.google.com/open?id=0ByhzM2YklhADNmk4cEN2MTA5U0E).
3. Add the downloaded pre-trained model to `Application/src/main/assets` folder in the repository.
4. Open the repository in Android Studio
5. Build the app on your device using Android Studio

## Working
The app is just a prototype, which uses our optimized and skimmed-down model from [image-caption-generator](https://github.com/neural-nuts/image-caption-generator), we also use a faster encoder CNN- Google's Inception v4.and finally use an end-to-end pre-trained model as balackbox in this app for quickly generating captions in real time.

Note: Due to lack of computation power our model is not very well trained.

Here is a quick preview of the app which was made using a slideshow running on a screen.

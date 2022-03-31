# Presidential Prediction 2022 by Facial Features

This project aims to showcase my basic understanding in Machine Learning Algorithms by taking the common topic of Filipino people during the elections. 

The 2022 Presidential Election is coming!
And we used the past Presidential Race aspirants' Facial Features to predict the next President.

![INTRO](/Screenshots/intro.png)

## Pre-requisites

I used this model to generate facial landmarks [68 Face Landmarks Shape Predictor](https://github.com/italojs/facial-landmarks-recognition/blob/d37b6a7426e98094e28fa99254e270a3e9b6d591/shape_predictor_68_face_landmarks.dat).

Scikit Image and Scikit Learn are common machine learning libraries mostly used for learning applications, translating well to more advanced libraries.
```bash
pip install -U scikit-image
pip install -U scikit-learn
```

## Methodology

The aspirants for the past 6 Presidential elections, since 1992, have been collected as the base data for the model. 
These are all generated manually using [Facial Data Generate Notebook](/FacialDataGenerate.ipynb) then encoded to [Presidential Features Excel](/PH_presidential_feature.xlsx)
Since data targets are unbalanced SMOTE has been implemented.

![Methodology](/Screenshots/methodology.png)

## Results

**76.03% Test Accuracy**  
**90.23% Train Accuracy**  
by Random Forest

kNN - 74.83%  
Decision Tree - 67.72%  
PCC Baseline Accuracy 65.34%  


![Win Rate](/Screenshots/winrate.png)

## Conclusion and Recommendations

The prediction is based mostly on Jawline Prominence produced by carefully selecting the ideal images of candidates. The model's accuracy relies on how well the dlib 68 points data predicts the facial landmarks.
Thus these are the things recommended to be improved:

- Apply Deep Learning Model to increase accuracy.
- Use larger datasets with other applications.
- Recreate the Ideal President Face.


## Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

## License
Distributed under the [MIT](https://choosealicense.com/licenses/mit/) License.

## Acknowledgement
Great appreciation to my teacher Sir. Elmer Joaquin and my teammates: Golden Domingo, Ivan Floyd Erer & Trisia Ann Luna.

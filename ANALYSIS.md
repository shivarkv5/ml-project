# ANALYSIS - TECHNICAL RESULTS of Test Dataset

## Linear Regression

For prediction, I have used "Temp_pre_7","Wind_pre_7","Hum_pre_7","Prec_pre_7" for X value and "fire_size" feature for Y value and used LinearRegression() function which gave the following results.

```
# Testing Set Values:
R2 value is : 0.010545398726775512
Mean Squared Error is : 471437993.5828763
```

## Random Forest Classifier

For classification, I have used the same features as above and used four metrics for evaluation:

```
# Testing Set Values:
Confusion Metrix: 
[[2694    2    0    0    1    1]
 [ 296  620    0    0    0    1]
 [  54    0  106    0    0    0]
 [  42    1    0   87    0    1]
 [ 121    0    0    1  305   12]
 [ 230    1    0    0    5  708]]
The Evalution metrics are as follows: 
Accuracy:  0.8546038948761581
Precision:  0.8830276745796406
Sensitivity:  0.8546038948761581
F1 Score:  0.8504237672224091
```

## Graphical Representation of Results after PCA + K-Means

![](https://github.com/44-599-MachineLearning-S21/project-machine-learning-s21-srkvodnala/blob/main/images/p4.png?raw=True)

![](https://github.com/44-599-MachineLearning-S21/project-machine-learning-s21-srkvodnala/blob/main/images/p5.png?raw=True)


## Challenges & Solutions

I had not faced much problem with prediction but while doing classification, SVM was running for a very, very long time. Hence I used Random Forest Classifier. I also used other models instead. 

## Limitations & Improvments

- Preprocessing of the data could have been better by arranging the values range wise.
- Cross Validation should be used for finer results.
- The accuracy and other metrics values should be above 90%, this means other models and algorithms can be used.

### IPYNB Notebooks: 

1. [Initial Exploration of Dataset](https://github.com/44-599-MachineLearning-S21/project-machine-learning-s21-srkvodnala/blob/main/initial_exploration.ipynb)

1. [Linear Regression](https://github.com/44-599-MachineLearning-S21/project-machine-learning-s21-srkvodnala/blob/main/linear_regression.ipynb)

1. [Classification](https://github.com/44-599-MachineLearning-S21/project-machine-learning-s21-srkvodnala/blob/main/Classification.ipynb)

1. [Data Analysis](https://github.com/44-599-MachineLearning-S21/project-machine-learning-s21-srkvodnala/blob/main/Data%20Analysis.ipynb)
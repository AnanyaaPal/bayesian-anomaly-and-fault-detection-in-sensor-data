<p align="center">
<img src="assets/TU_Dortmund_logo.png">
</p>
<p align="center">
<img src="assets/fakultaet_statistik_logo.png" height="50" >
</p>

## Bayesian Activity Anomaly (and Fault) Detection Using Wearable Sensor Data

This project is carried out as a part of the graded module: 
On the Theory and Practice of Monte Carlo Simulations (Methods, 4.5 ECTS)

Further, it is classified as an application-oriented topic.

The goal is to implement MCMC for Naïve Bayes classification to the following binary classfication dataset, and to quantify prediction uncertainity. 

### Goal of the project: Detect movement vs no movement from the sensor data.
In the dataset, there are 6 ADL (Activities of Daily Living) - Standing, Sitting, Laying Down, Walking, Walking Upstairs and Walking Downstairs. 

Of these 6 ADLs, one can define:
- Static Activites: Standing, Sitting, Laying Down 
- Dynamic Activities: Walking, Walking Upstairs, Walking Downstairs

Detailed information about the dataset can be found [here](data/README.txt).

## Specifics of applying the Naïve Bayes algorithm 
We would classify the 6 ADLs into two classes from [activity labels](data/train/activity_labels.txt):
- Class 1- Static Activities (includes activities "Standing", "Sitting", "Laying Down") with class labels 4, 5, 6
- Class 2- Dynamic Activities (includes activities "Walking", "Walking Upstairs", "Walking Downstairs") with class labels 1, 2, 3

Our goal would be to apply Gaussian Naive Bayes to our use case, since on the first descriptive look, it satifies the following (pre-)conditions of G.N.B:
- features are continuous/numeric
- no need for feature binning
- supports binary classification

## Gaussian Naïve Bayes Algorithm
### Pre-checks:
- G.N.B works best when:
    - feature distributions are roughly unimodal per class.
    - independence assumption is not riughly violated.
- Plot a histogram per feature per class and normality plots.  




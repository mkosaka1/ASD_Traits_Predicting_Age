# Module 2 Final Project
By: Muriel Kosaka

## Introduction

Autism Spectrum Disorder (ASD) is a neurodevelopmental disorder that affects communication and behavior. Early detection of ASD is beneficial for both the parent and the child. In this final project, I examined a dataset provided on Kaggle that included individual characteristics and features to determine ASD traits. These features included the QChat-10 which are 10 questions about the child’s behavior, and then individual characteristics such as sex, ethnicity, whether or not the child was born with Jaundice, if an immediate family member has ASD, and who completed the test. Scores 4 and above on the QChat-10 indicated that the child had traits of ASD. Using the features provided, I aimed to create a linear regression model to predict age.
If we can predict the age of toddlers with traits of ASD, this can help parents look out for the early signs and have their child tested and receive treatment earlier.

## Process

1) See **project_regression.ipynb**: Using the dataset, Toddler Autism dataset July 2018.csv from Kaggle, I cleaned the data, conducted necessary EDA and created three multi-linear regression models using feature selection methods: 

    - Using questions A1-A10 from QChat-10 to predict age
    - Using interactions of questions A1-A10 from QChat-10 to 
        predict age
    - Using individual characteristics to predict age
        
2) See **project_hypothesis_test.ipynb**: Then based off my results from the linear regression models, I conducted three hypothesis tests:

    - Independent samples t-test between Sex on QChat-10 
        scores: results were not significant. 
    - Independent samples t-test between toddlers who 
        were/were not born with Jaundice on QChat-10 scores: 
        results were not significant.
    - One way ANOVA between ethnicities on QChat-10 scores: 
        results were significant between White European and 
        Asian.


## Libraries

### Data Collection:

- Pandas

### Data Cleaning and Visualization:

- Matplotlib
- Seaborn
- Pandas
- SciPy
- Sklearn
- NumPy
- Statsmodels

## Findings and Limitations

When looking to predict age it is best to use the individual characteristics, although it will over-estimate by 7.17 months. QChat-10 scores best predict age, as QChat-10 scores increase by 1, age goes down by 1.30 months. There is no significant difference in average qchat-10 scores between those who were/were not born with jaundice (* *p* * = 0.72) and between sex (* *p* * = 0.09). White european and asian toddlers had the most significant difference in average qchat-10 scores (* *p* * < 0.05). 

Limitations of our model include who was filling out the survey for the toddlers, there may have been some bias in the responses, e.g. social desirability bias.

Future models should include data such as extremely preterm babies, presence of other disorders, and parental information such as age and the presence of obesity and/or diabetes.








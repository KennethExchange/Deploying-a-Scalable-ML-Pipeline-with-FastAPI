# Model Card

For additional information see the Model Card paper: https://arxiv.org/pdf/1810.03993.pdf

## Model Details
This is a Random Forest classification model using publicly 
available Census Bureau distributed by UC Irvine.
- Person or organization developing model:  This model created by 
Kenneth Exchange as per of the following course 
project:  Deploying-a-Scalable-ML-Pipeline-with-FastAPI.
- Model date:  This model was created on Nov 27, 2024.
- Model version:  1.0.0
- Model Type:  Random Forest
- Training performed using sklearn's RandomForestClassifier.
- This model is created as part of Project 2 from section 13 of 
WGU / Udacity course:  D501 Machine Learning DevOps.
- License:  Copyright © 2012 - 2020, Udacity, Inc.  See 
LICENSE.txt for details.

## Intended Use
- Primary intended uses:  To identify and compare metrics based on 
various slices of the provided census data.
- Primary intended users:  Udacity project reviewers.

## Training Data
Preprocessing of categorical data performed using OneHotEncoder and 
LabelBinarizer from sklearn.preprocessing.  Preprocessing details 
found in ml\data.py.

Note: In order to have reproducibility for this project, the 
random_state was set to 42.

## Evaluation Data
This dataset is provided online by UC Irvine and can be found 
at: https://archive.ics.uci.edu/dataset/20/census+income. Per the 
UCI website for this data extraction was done by Barry Becker from 
the 1994 Census database.  A set of reasonably clean records was 
extracted using the following conditions: ((AAGE>16) && (AGI>100) 
&& (AFNLWGT>1)&& (HRSWK>0)).  (https://archive.ics.uci.edu/dataset/20/census+income)

## Metrics
Metrics used for this model include the precision, recall, and F1 
score.  

The performance per these metrics are as follows:
- Precision: 0.7739
- Recall: 0.6305
- F1: 0.6949

Performance per each slice of data can be found in the following 
file:  slice_output.txt.There are approximately 198 slices 
represented in this file.

## Ethical Considerations
This data is publicly available and distributed by UC Irvine.  This 
data does not include personally identifying information or other 
sensitive data.  This data was gathered in 1994 and may not be 
representative of census data for any other year.

## Caveats and Recommendations
Given the current year of 2024, it would be recommended that a 
more current dataset be used for this model in order to maximize 
the model's relevance.



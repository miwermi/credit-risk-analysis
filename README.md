# Credit Risk Analysis

## Overview
The purpose of this analysis is to use different machine learning methods to review loan data and analyze lending risk -- and to ascertain the differences and value in each of the methods. Using Python and the SciKit-Learn Library to build and evaluate several models, the results below reveal the variation in model outcomes and predicted risk. The final summary compares the strengths and weakness of each model.

## Results
### Oversampling
- Accuracy Score: 66% (0.6620175698580149)
- Confusion Matrix

  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | Actual High-Risk (0) | 	73 |   	 28 |
  | Actual Low-Risk (1) | 6820 | 	10284 |

- Imbalanced Classification Report

### Oversampling with SMOTE
- Accuracy Score: 66% (0.6568196079430206)
- Confusion Matrix

  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | Actual High-Risk (0) | 	62 | 	  39 |
  | Actual Low-Risk (1) | 5135 | 11969 |

- Imbalanced Classification Report

### Undersampling
- Accuracy Score: 54% (0.5442661782548694)
- Confusion Matrix

  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | Actual High-Risk (0) | 	 70 |   	31 |
  | Actual Low-Risk (1) | 10340 | 	6764 |
  
- Imbalanced Classification Report

### Combination (Over+Under) Sampling with SMOTEENN
- Accuracy Score: 65% (0.6461148570422992)
- Confusion Matrix
  	
  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | Actual High-Risk (0) |	73 |	  28 |
  | Actual Low-Risk (1) |	7364 |	9740 |
  
- Imbalanced Classification Report

### Ensemble Learning with Random Forest
- Accuracy Score: 79% (0.7885466545953005) 
- Confusion Matrix:
  	
  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | Actual High-Risk (0) | 	71 |    30 | 
  | Actual Low-Risk (1) | 2153 | 14951 | 
  
- Imbalanced Classification Report

### Ensemble Learning with Easy Ensemble
- Accuracy Score: 93% (0.9316600714093861)
- Confusion Matrix

  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | Actual High-Risk (0) | 93 |     8 |
  | Actual Low-Risk (1) | 983 | 16121 |
  
- Imbalanced Classification Report

## Summary
Summarizing the results of the machine learning models, and a recommendation on the model to use, if any. Justified reasoning.

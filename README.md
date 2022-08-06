# Credit Risk Analysis

## Overview
The purpose of this analysis is to use different machine learning methods to review loan data and analyze lending risk -- and to ascertain the differences and value in each of the methods. Using Python and the SciKit-Learn Library to build and evaluate several models, the results below reveal the variation in model outcomes and predicted risk. The final summary compares the strengths and weakness of each model.

## Results
Because all machine learning techniques are attempting to predict future outcomes based on already existing data, there is no absolute view of the future and no method can predict it perfectly. Six methods were use to analyze loan data from LendingClub, a popular lending services company. Each is listed below with the typical drawback of that method and the results of each analysis.

### Oversampling
- Typical drawback of this method: Oversampling is prone to overfitting. Overfitting often fails to predict future data reliably because results correspond too closely or exactly to the training and test sets.
- Accuracy Score: **66%** (0.6620175698580149)
- Confusion Matrix:

  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | **Actual High-Risk (0)** | 	73 |   	 28 |
  | **Actual Low-Risk (1)** | 6820 | 	10284 |

- Imbalanced Classification Report:
<img src="https://github.com/miwermi/credit-risk-analysis/blob/main/graphics/oversampling.jpg" alt ="graphic">


### Oversampling with SMOTE (Synthetic Minority Oversampling Technique)
- Typical drawback of this method: SMOTE is still oversampling and is still prone to overfitting. Using the synthetic method can help to overcome class imbalances and lessen the exactness of outcome dependency on minority classes.
- Accuracy Score: **66%** (0.6568196079430206)
- Confusion Matrix:

  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | **Actual High-Risk (0)** | 	62 | 	  39 |
  | **Actual Low-Risk (1)** | 5135 | 11969 |

- Imbalanced Classification Report:
<img src="https://github.com/miwermi/credit-risk-analysis/blob/main/graphics/smote.jpg" alt ="graphic">

### Undersampling
- Typical drawback of this method: Undersampling tries to balance data by keeping all minority classes. Undersampling can often lower accuracy for datasets having minority classes not closely correlated to the majority classes.
- Accuracy Score: **54%** (0.5442661782548694)
- Confusion Matrix: 

  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | **Actual High-Risk (0)**  | 	 70 |   	31 |
  | **Actual Low-Risk (1)** | 10340 | 	6764 |

- Imbalanced Classification Report:
<img src="https://github.com/miwermi/credit-risk-analysis/blob/main/graphics/undersampling.jpg" alt ="graphic">

### Combination (Over+Under) Sampling with SMOTEENN (Edited Nearest Neighbors)
- Typical drawback of this method: Using SMOTE to oversample via synthetic methods to help overcome class imbalances -- and then also ENN and choose more relevant minority classes may not make any relevant gains in predictive accuracy but it may provied quality comparison value.
- Accuracy Score: **65%** (0.6461148570422992)
- Confusion Matrix
  	
  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | **Actual High-Risk (0)**  |	73 |	  28 |
  | **Actual Low-Risk (1)** |	7364 |	9740 |

- Imbalanced Classification Report:
<img src="https://github.com/miwermi/credit-risk-analysis/blob/main/graphics/smoteenn.jpg" alt ="graphic">

### Ensemble Learning with Random Forest
- Typical drawback of this method: Complexity. Ensemble learning methods use combined methods to predict and are best used when *performance* on a predictive modeling project is the *most important outcome*. The reasoning for the higher performance is not always easy to decipher though, and depending on the size of the dataset, ensemble modeling can end up using far more resources.
- Accuracy Score: **79%** (0.7885466545953005) 
- Confusion Matrix:
  	
  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | **Actual High-Risk (0)**  | 	71 |    30 | 
  | **Actual Low-Risk (1)** | 2153 | 14951 | 
  
- Imbalanced Classification Report:
<img src="https://github.com/miwermi/credit-risk-analysis/blob/main/graphics/randomforest.jpg" alt ="graphic">

### Ensemble Learning with Easy Ensemble
- Typical drawback of this method: Complexity. Ensemble learning methods use combined methods to predict and are best used when *performance* on a predictive modeling project is the *most important outcome*. The reasoning for the higher performance is not always easy to decipher though, and depending on the size of the dataset, ensemble modeling can end up using far more resources. (same as above)
- Accuracy Score: **93%** (0.9316600714093861)
- Confusion Matrix

  |  | Predicted High-Risk (0) | Predicted Low-Risk (1) |
  | ---: | ---: | ---: |
  | **Actual High-Risk (0)**  | 93 |     8 |
  | **Actual Low-Risk (1)** | 983 | 16121 |
  
- Imbalanced Classification Report:
<img src="https://github.com/miwermi/credit-risk-analysis/blob/main/graphics/easyensemble.jpg" alt ="graphic">

## Summary
Summarizing the results of the machine learning models, and a recommendation on the model to use, if any. Justified reasoning.

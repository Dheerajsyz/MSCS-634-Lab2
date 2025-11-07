# MSCS 634 Lab 2 - KNN and RNN Classifiers

## Project Overview

This lab analyzes KNN and RNN classifiers using the Wine Dataset from sklearn to understand how different parameter values affect classification accuracy.

## Dataset

- **Source**: sklearn.datasets.load_wine()
- **Classes**: 3 wine types
- **Features**: 13 chemical properties
- **Instances**: 178 samples
- **Split**: 80% training, 20% testing

## Implementation

### KNN Classifier
Tested with k values: 1, 5, 11, 15, 21

**Results:**
- k=1: 97.22% accuracy
- k=5: 97.22% accuracy
- k=11: 100.00% accuracy
- k=15: 100.00% accuracy
- k=21: 100.00% accuracy

### RNN Classifier
Tested with radius values: 350, 400, 450, 500, 550, 600
<img width="1390" height="490" alt="image" src="https://github.com/user-attachments/assets/db8d3c9c-817c-46af-b7c0-b46fae2859f6" />


**Results:**
- All radius values: 38.89% accuracy

## Key Findings

**KNN Performance:**
- Lower k values (1, 5) showed good accuracy but potential for overfitting
- Higher k values (11, 15, 21) achieved perfect accuracy on the test set
- Performance improved as k increased, stabilizing at k=11

**RNN Performance:**
- Consistent accuracy across all radius values tested
- Lower performance indicates radius values may need adjustment
- Suggests data points are either too close or too far for the chosen radius range

**Model Comparison:**
- KNN performed significantly better on this dataset
- KNN achieved 97-100% accuracy vs RNN's 38.89%
- Feature scaling with StandardScaler was critical for both models


## Project Structure

```
lab2/
├── .github/
│   └── copilot-instructions.md
├── lab2_knn_rnn_analysis.ipynb
├── README.md
└── requirements.txt
```


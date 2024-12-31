# Custom K-Nearest Neighbors (KNN) Algorithm

This project implements a custom **K-Nearest Neighbors (KNN)** algorithm and compares it with Scikit-learn's KNN using 10-fold cross-validation across three datasets: **Hayes-Roth**, **Car Evaluation**, and **Breast Cancer**. The performance was assessed using accuracy scores and hypothesis testing via a paired T-test.

## Features
1. **Custom KNN Implementation**:
   - Built from scratch, calculates distances using:
     - Euclidean Distance
     - Manhattan Distance
     - Hamming Distance
   - Weighted distance metrics for improved predictions.

2. **Scikit-learn KNN Comparison**:
   - Uses Scikit-learn’s KNN with identical parameters for accuracy benchmarking.

3. **Cross-Validation**:
   - 10-fold cross-validation was applied to evaluate model robustness and mean accuracy.

4. **Hypothesis Testing**:
   - Paired T-test conducted to determine statistical significance of differences in model performance.

## Results
### Hayes-Roth Dataset:
- **Custom KNN** achieved a mean accuracy of 66% using Manhattan distance.
- **Scikit-learn KNN** scored 57% accuracy.
- **Hypothesis Test**: P-value showed no statistically significant difference in performance.

### Car Evaluation Dataset:
- **Custom KNN** outperformed Scikit-learn, showing a higher accuracy using Manhattan distance.
- **Hypothesis Test**: No significant difference in performance according to P-value.

### Breast Cancer Dataset:
- **Custom KNN** and **Scikit-learn KNN** achieved nearly identical accuracies (~66%).
- **Hypothesis Test**: Confirmed no significant difference between the two models.

## Key Insights
- Both implementations showed comparable results, validating the reliability of the custom KNN algorithm.
- The choice of distance metric and number of neighbors (`K`) greatly influences model accuracy.
- Manhattan distance consistently produced better results across datasets.

## Requirements
- Python 3.x
- Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`

## Usage
1. Place the datasets (`Hayes-Roth`, `Car Evaluation`, and `Breast Cancer`) in the project directory.
2. Run the provided Python file to execute the custom KNN algorithm and Scikit-learn comparison.
3. View the accuracy scores, confusion matrices, and hypothesis test results.

## Conclusion
This project demonstrates the reliability and versatility of KNN for classification tasks. While Scikit-learn provides a robust baseline, custom implementation offers flexibility for fine-tuning distance metrics and weighting schemes.

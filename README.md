# Project Title: HW1_MatanOz_DinKosberg_final

## Description
This project involves various tasks and analyses related to HW1 for the course.

## Table of Contents
1. ## Q4 - Conclusions
2. ### Conclusions for the Original Dataset Classification Results
3. ### Conclusions for the Averaged Dataset Classification Results
4. ### Comparison between Original and Averaged Dataset Classification Results
5. ### Conclusions for the PCA Reduced Dataset Classification Results
6. ### Conclusions for the Block Averaged Dataset Classification Results
7. ### Comparison between Block Averaged and PCA Reduced Dataset Classification Results
8. ### Conclusions for the Undersampled Dataset Classification Results
9. ### Conclusions for the Oversampled Dataset Classification Results
10. ### Comparison between Oversampled and Undersampled Dataset Classification Results

## 1. ## Q4 - Conclusions

### Based on the histograms:

- The class distribution is fairly balanced, with each class having a similar number of images.
- The average number of white pixels per image varies across classes, indicating differences in digit complexity and the amount of ink used to draw different digits.
- The standard deviation of white pixels indicates that some classes have more variability in how they are written than others. For example, digits like 1 might have less variability compared to digits like 8.
- The average number of non-white pixels complements the average number of white pixels, confirming the pixel density patterns observed.

## 2. ### Conclusions for the Original Dataset Classification Results

#### Performance Metrics
- **Accuracy**: 0.9788 - This indicates that 97.88% of the predictions made by the model are correct, demonstrating very high overall performance.
- **Precision**: 0.978672 - High precision indicates a low false positive rate, meaning that when the model predicts a positive class, it is usually correct.
- **Recall**: 0.978737 - High recall indicates that the model correctly identifies a high proportion of actual positives.
- **F1 Score**: 0.978650 - The F1 score, which balances precision and recall, suggests the model has an excellent balance between these two metrics.
- **Balanced Accuracy**: 0.978737 - Balanced accuracy suggests that the model is equally good at predicting both positive and negative classes.
- **Specificity**: 0.978737 - High specificity indicates that the model correctly identifies a high proportion of actual negatives.
- **Sensitivity**: 0.978737 - Sensitivity, equivalent to recall, shows the model's ability to correctly identify true positives.

#### Confusion Matrix Analysis

The confusion matrix provides a detailed breakdown of actual versus predicted classes:

- **Class 0**: 973 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1126 out of 1135 instances were correctly predicted.
- **Class 2**: 1010 out of 1032 instances were correctly predicted.
- **Class 3**: 973 out of 1010 instances were correctly predicted.
- **Class 4**: 968 out of 982 instances were correctly predicted.
- **Class 5**: 877 out of 892 instances were correctly predicted.
- **Class 6**: 946 out of 958 instances were correctly predicted.
- **Class 7**: 1001 out of 1028 instances were correctly predicted.
- **Class 8**: 936 out of 974 instances were correctly predicted.
- **Class 9**: 978 out of 1009 instances were correctly predicted.

#### Error Analysis

- **Class 0**: Very high correct prediction rate with only 7 misclassifications.
- **Class 1**: Few misclassifications, with 4 instances predicted as class 2 and minor errors.
- **Class 2**: Slightly higher misclassifications with instances predicted as classes 1, 3, and 4.
- **Class 3**: Higher misclassification rate with 9 instances predicted as class 2 and others.
- **Class 4**: Few misclassifications, with most instances correctly identified.
- **Class 5**: Some misclassifications into classes 0 and 3, but overall good performance.
- **Class 6**: Very high correct prediction rate with minimal errors.
- **Class 7**: Some misclassifications into classes 1, 2, and 8.
- **Class 8**: Higher misclassifications into classes 3 and 5.
- **Class 9**: Some misclassifications, but overall high correct prediction rate.

#### Detailed Observations
1. **High Correct Prediction Rates**: Most classes have a high number of correct predictions, demonstrating the model's effectiveness.
2. **Misclassification Patterns**: Misclassifications are generally low and spread across different classes, indicating some areas for improvement.
3. **Class-Specific Observations**: Classes 3, 7, and 8 show relatively higher misclassification rates compared to other classes.

#### Conclusion

The neural network model trained on the original dataset demonstrates excellent performance across all metrics, with very high accuracy, precision, recall, and F1 score. The balanced accuracy suggests that the model treats both positive and negative classes equally well. The confusion matrix reveals a high true positive rate for most classes, indicating strong classification ability.

However, there are some areas for improvement, particularly in classes 3, 7, and 8, where misclassifications are relatively higher. These findings suggest that while the model performs exceptionally well, it may benefit from further tuning or additional data to further reduce errors in these specific classes.

Overall, the model is highly effective and reliable for the given classification task, providing strong performance metrics and a balanced approach to class prediction.

## 3. ### Conclusions for the Averaged Dataset Classification Results

#### Performance Metrics
- **Accuracy**: 0.9776 - This indicates that 97.76% of the predictions made by the model are correct, demonstrating very high overall performance.
- **Precision**: 0.977643 - High precision indicates a low false positive rate, meaning that when the model predicts a positive class, it is usually correct.
- **Recall**: 0.977462 - High recall indicates that the model correctly identifies a high proportion of actual positives.
- **F1 Score**: 0.977489 - The F1 score, which balances precision and recall, suggests the model has an excellent balance between these two metrics.
- **Balanced Accuracy**: 0.977462 - Balanced accuracy suggests that the model is equally good at predicting both positive and negative classes.
- **Specificity**: 0.977462 - High specificity indicates that the model correctly identifies a high proportion of actual negatives.
- **Sensitivity**: 0.977462 - Sensitivity, equivalent to recall, shows the model's ability to correctly identify true positives.

#### Confusion Matrix Analysis

The confusion matrix provides a detailed breakdown of actual versus predicted classes:

- **Class 0**: 968 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1120 out of 1135 instances were correctly predicted.
- **Class 2**: 992 out of 1032 instances were correctly predicted.
- **Class 3**: 990 out of 1010 instances were correctly predicted.
- **Class 4**: 950 out of 982 instances were correctly predicted.
- **Class 5**: 869 out of 892 instances were correctly predicted.
- **Class 6**: 948 out of 958 instances were correctly predicted.
- **Class 7**: 1017 out of 1028 instances were correctly predicted.
- **Class 8**: 935 out of 974 instances were correctly predicted.
- **Class 9**: 987 out of 1009 instances were correctly predicted.

#### Error Analysis

- **Class 0**: Very high correct prediction rate with only 12 misclassifications.
- **Class 1**: Few misclassifications, with 11 instances predicted as other classes.
- **Class 2**: Slightly higher misclassifications with instances predicted as classes 3 and 8.
- **Class 3**: Higher misclassification rate with 20 instances predicted as other classes.
- **Class 4**: Some misclassifications into other classes, particularly class 9.
- **Class 5**: Some misclassifications into classes 3 and 0, but overall good performance.
- **Class 6**: Very high correct prediction rate with minimal errors.
- **Class 7**: Some misclassifications into classes 1, 2, and 8.
- **Class 8**: Higher misclassifications into classes 3 and 5.
- **Class 9**: Some misclassifications, but overall high correct prediction rate.

#### Detailed Observations
1. **High Correct Prediction Rates**: Most classes have a high number of correct predictions, demonstrating the model's effectiveness.
2. **Misclassification Patterns**: Misclassifications are generally low and spread across different classes, indicating some areas for improvement.
3. **Class-Specific Observations**: Classes 3, 4, and 8 show relatively higher misclassification rates compared to other classes.

#### Conclusion

The neural network model trained on the averaged dataset demonstrates excellent performance across all metrics, with very high accuracy, precision, recall, and F1 score. The balanced accuracy suggests that the model treats both positive and negative classes equally well. The confusion matrix reveals a high true positive rate for most classes, indicating strong classification ability.

However, there are some areas for improvement, particularly in classes 3, 4, and 8, where misclassifications are relatively higher. These findings suggest that while the model performs exceptionally well, it may benefit from further tuning or additional data to further reduce errors in these specific classes.

Overall, the model is highly effective and reliable for the given classification task, providing strong performance metrics and a balanced approach to class prediction.

## 4. ### Comparison between Original and Averaged Dataset Classification Results

#### Performance Metrics
| Metric              | Original Dataset | Averaged Dataset |
|---------------------|------------------|------------------|
| Accuracy            | 0.978800         | 0.977600         |
| Precision           | 0.978672         | 0.977643         |
| Recall              | 0.978737         | 0.977462         |
| F1 Score            | 0.978650         | 0.977489         |
| Balanced Accuracy   | 0.978737         | 0.977462         |
| Specificity         | 0.978737         | 0.977462         |
| Sensitivity         | 0.978737         | 0.977462         |

#### Key Observations

1. **Accuracy**:
   - The original dataset achieves slightly higher accuracy (0.978800) compared to the averaged dataset (0.977600), indicating that the original dataset model makes fewer overall errors.

2. **Precision**:
   - Precision is slightly higher for the original dataset (0.978672) compared to the averaged dataset (0.977643). This suggests that the original dataset model is more effective in minimizing false positives.

3. **Recall**:
   - Recall is also marginally higher for the original dataset (0.978737) compared to the averaged dataset (0.977462). This indicates that the original dataset model is slightly better at correctly identifying true positives.

4. **F1 Score**:
   - The F1 score, which balances precision and recall, is higher for the original dataset (0.978650) than for the averaged dataset (0.977489). This suggests that the original dataset model has a better balance between precision and recall.

5. **Balanced Accuracy, Specificity, Sensitivity**:
   - All these metrics are higher for the original dataset, indicating a more balanced performance in handling both positive and negative classes.

#### Confusion Matrix Analysis

**Original Dataset**:
- **Class 0**: 973 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1126 out of 1135 instances were correctly predicted.
- **Class 2**: 1010 out of 1032 instances were correctly predicted.
- **Class 3**: 973 out of 1010 instances were correctly predicted.
- **Class 4**: 968 out of 982 instances were correctly predicted.
- **Class 5**: 877 out of 892 instances were correctly predicted.
- **Class 6**: 946 out of 958 instances were correctly predicted.
- **Class 7**: 1001 out of 1028 instances were correctly predicted.
- **Class 8**: 936 out of 974 instances were correctly predicted.
- **Class 9**: 978 out of 1009 instances were correctly predicted.

**Averaged Dataset**:
- **Class 0**: 968 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1120 out of 1135 instances were correctly predicted.
- **Class 2**: 992 out of 1032 instances were correctly predicted.
- **Class 3**: 990 out of 1010 instances were correctly predicted.
- **Class 4**: 950 out of 982 instances were correctly predicted.
- **Class 5**: 869 out of 892 instances were correctly predicted.
- **Class 6**: 948 out of 958 instances were correctly predicted.
- **Class 7**: 1017 out of 1028 instances were correctly predicted.
- **Class 8**: 935 out of 974 instances were correctly predicted.
- **Class 9**: 987 out of 1009 instances were correctly predicted.

#### Detailed Observations

1. **Misclassification Rates**:
   - The original dataset has fewer misclassifications across most classes compared to the averaged dataset.
   - The averaged dataset shows more misclassifications in classes 4 and 8.

2. **Class 0 Performance**:
   - The original dataset model correctly predicted 973 out of 980 instances for class 0, whereas the averaged dataset model correctly predicted 968 out of 980 instances.

3. **Class 1 Performance**:
   - The original dataset model correctly predicted 1126 out of 1135 instances, while the averaged dataset model correctly predicted 1120 out of 1135 instances.

4. **Class 4 and Class 8 Performance**:
   - Class 4 and class 8 show more misclassifications in the averaged dataset compared to the original dataset.

5. **Overall Misclassification Trends**:
   - The original dataset model shows a more even distribution of correct predictions and fewer misclassifications across all classes.

#### Conclusion

The neural network model trained on the original dataset outperforms the model trained on the averaged dataset in terms of accuracy, precision, recall, F1 score, and balanced accuracy. The original dataset model demonstrates a more balanced and effective performance across all classes, with fewer misclassifications.

The averaged dataset model, while still performing well, shows higher misclassification rates, particularly in classes 4 and 8. These higher misclassifications suggest that the averaging approach might have introduced slight noise or reduced the model's ability to generalize as effectively as the original dataset.

In summary, the original dataset model is preferable due to its higher accuracy and balanced performance, making it more reliable for the given classification task. The averaged dataset model, although effective, requires further tuning or alternative strategies to mitigate the introduced noise and improve its generalization capabilities.

## 5. ### Conclusions for the PCA Reduced Dataset Classification Results

#### Performance Metrics
- **Accuracy**: 0.9715 - This indicates that 97.15% of the predictions made by the model are correct, demonstrating high overall performance.
- **Precision**: 0.971375 - High precision indicates a low false positive rate, meaning that when the model predicts a positive class, it is usually correct.
- **Recall**: 0.971114 - High recall indicates that the model correctly identifies a high proportion of actual positives.
- **F1 Score**: 0.971199 - The F1 score, which balances precision and recall, suggests the model has a good balance between these two metrics.
- **Balanced Accuracy**: 0.971114 - Balanced accuracy suggests that the model is equally good at predicting both positive and negative classes.
- **Specificity**: 0.971114 - High specificity indicates that the model correctly identifies a high proportion of actual negatives.
- **Sensitivity**: 0.971114 - Sensitivity, equivalent to recall, shows the model's ability to correctly identify true positives.

#### Confusion Matrix Analysis

The confusion matrix provides a detailed breakdown of actual versus predicted classes:

- **Class 0**: 967 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1127 out of 1135 instances were correctly predicted.
- **Class 2**: 992 out of 1032 instances were correctly predicted.
- **Class 3**: 988 out of 1010 instances were correctly predicted.
- **Class 4**: 959 out of 982 instances were correctly predicted.
- **Class 5**: 856 out of 892 instances were correctly predicted.
- **Class 6**: 936 out of 958 instances were correctly predicted.
- **Class 7**: 1000 out of 1028 instances were correctly predicted.
- **Class 8**: 922 out of 974 instances were correctly predicted.
- **Class 9**: 968 out of 1009 instances were correctly predicted.

#### Error Analysis

- **Class 0**: Very high correct prediction rate with only 13 misclassifications.
- **Class 1**: Few misclassifications, with 8 instances predicted as other classes.
- **Class 2**: Slightly higher misclassifications with instances predicted as classes 3 and 8.
- **Class 3**: Higher misclassification rate with 20 instances predicted as other classes.
- **Class 4**: Some misclassifications into other classes, particularly class 9.
- **Class 5**: Some misclassifications into classes 3 and 0, but overall good performance.
- **Class 6**: Very high correct prediction rate with minimal errors.
- **Class 7**: Some misclassifications into classes 1, 2, and 8.
- **Class 8**: Higher misclassifications into classes 3 and 5.
- **Class 9**: Some misclassifications, but overall high correct prediction rate.

#### Detailed Observations
1. **High Correct Prediction Rates**: Most classes have a high number of correct predictions, demonstrating the model's effectiveness.
2. **Misclassification Patterns**: Misclassifications are generally low and spread across different classes, indicating some areas for improvement.
3. **Class-Specific Observations**: Classes 3, 4, and 8 show relatively higher misclassification rates compared to other classes.

#### Conclusion

The neural network model trained on the PCA reduced dataset demonstrates high performance across all metrics, with high accuracy, precision, recall, and F1 score. The balanced accuracy suggests that the model treats both positive and negative classes equally well. The confusion matrix reveals a high true positive rate for most classes, indicating strong classification ability.

However, there are some areas for improvement, particularly in classes 3, 4, and 8, where misclassifications are relatively higher. These findings suggest that while the model performs very well, it may benefit from further tuning or additional data to further reduce errors in these specific classes.

Overall, the model is highly effective and reliable for the given classification task, providing strong performance metrics and a balanced approach to class prediction.

## 6. ### Conclusions for the Block Averaged Dataset Classification Results

#### Performance Metrics
- **Accuracy**: 0.9698 - This indicates that 96.98% of the predictions made by the model are correct, demonstrating high overall performance.
- **Precision**: 0.969890 - High precision indicates a low false positive rate, meaning that when the model predicts a positive class, it is usually correct.
- **Recall**: 0.969396 - High recall indicates that the model correctly identifies a high proportion of actual positives.
- **F1 Score**: 0.969540 - The F1 score, which balances precision and recall, suggests the model has a good balance between these two metrics.
- **Balanced Accuracy**: 0.969396 - Balanced accuracy suggests that the model is equally good at predicting both positive and negative classes.
- **Specificity**: 0.969396 - High specificity indicates that the model correctly identifies a high proportion of actual negatives.
- **Sensitivity**: 0.969396 - Sensitivity, equivalent to recall, shows the model's ability to correctly identify true positives.

#### Confusion Matrix Analysis

The confusion matrix provides a detailed breakdown of actual versus predicted classes:

- **Class 0**: 968 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1125 out of 1135 instances were correctly predicted.
- **Class 2**: 1004 out of 1032 instances were correctly predicted.
- **Class 3**: 983 out of 1010 instances were correctly predicted.
- **Class 4**: 951 out of 982 instances were correctly predicted.
- **Class 5**: 861 out of 892 instances were correctly predicted.
- **Class 6**: 933 out of 958 instances were correctly predicted.
- **Class 7**: 1005 out of 1028 instances were correctly predicted.
- **Class 8**: 908 out of 974 instances were correctly predicted.
- **Class 9**: 960 out of 1009 instances were correctly predicted.

#### Error Analysis

- **Class 0**: Very high correct prediction rate with only 12 misclassifications.
- **Class 1**: Few misclassifications, with 10 instances predicted as other classes.
- **Class 2**: Slightly higher misclassifications with instances predicted as classes 3 and 8.
- **Class 3**: Higher misclassification rate with 27 instances predicted as other classes.
- **Class 4**: Some misclassifications into other classes, particularly class 9.
- **Class 5**: Some misclassifications into classes 3 and 0, but overall good performance.
- **Class 6**: Very high correct prediction rate with minimal errors.
- **Class 7**: Some misclassifications into classes 1, 2, and 8.
- **Class 8**: Higher misclassifications into classes 3 and 5.
- **Class 9**: Some misclassifications, but overall high correct prediction rate.

#### Detailed Observations
1. **High Correct Prediction Rates**: Most classes have a high number of correct predictions, demonstrating the model's effectiveness.
2. **Misclassification Patterns**: Misclassifications are generally low and spread across different classes, indicating some areas for improvement.
3. **Class-Specific Observations**: Classes 3, 4, and 8 show relatively higher misclassification rates compared to other classes.

#### Conclusion

The neural network model trained on the block averaged dataset demonstrates high performance across all metrics, with high accuracy, precision, recall, and F1 score. The balanced accuracy suggests that the model treats both positive and negative classes equally well. The confusion matrix reveals a high true positive rate for most classes, indicating strong classification ability.

However, there are some areas for improvement, particularly in classes 3, 4, and 8, where misclassifications are relatively higher. These findings suggest that while the model performs very well, it may benefit from further tuning or additional data to further reduce errors in these specific classes.

Overall, the model is highly effective and reliable for the given classification task, providing strong performance metrics and a balanced approach to class prediction.

## 7. ### Comparison between Block Averaged and PCA Reduced Dataset Classification Results

#### Performance Metrics
| Metric              | Block Averaged Dataset | PCA Reduced Dataset |
|---------------------|------------------------|---------------------|
| Accuracy            | 0.969800               | 0.971500            |
| Precision           | 0.969890               | 0.971375            |
| Recall              | 0.969396               | 0.971114            |
| F1 Score            | 0.969540               | 0.971199            |
| Balanced Accuracy   | 0.969396               | 0.971114            |
| Specificity         | 0.969396               | 0.971114            |
| Sensitivity         | 0.969396               | 0.971114            |

#### Key Observations
1. **Accuracy**:
   - The PCA Reduced model has a slightly higher accuracy (0.971500) compared to the Block Averaged model (0.969800).

2. **Precision**:
   - Precision is marginally higher for the PCA Reduced model (0.971375) compared to the Block Averaged model (0.969890).

3. **Recall**:
   - Recall is also higher for the PCA Reduced model (0.971114) compared to the Block Averaged model (0.969396).

4. **F1 Score**:
   - The F1 score, which balances precision and recall, is higher for the PCA Reduced model (0.971199) than for the Block Averaged model (0.969540).

5. **Balanced Accuracy, Specificity, Sensitivity**:
   - All these metrics are higher for the PCA Reduced model, indicating a more balanced performance in handling both positive and negative classes.

#### Confusion Matrix Analysis

**Block Averaged Dataset**:
- **Class 0**: 968 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1125 out of 1135 instances were correctly predicted.
- **Class 2**: 1004 out of 1032 instances were correctly predicted.
- **Class 3**: 983 out of 1010 instances were correctly predicted.
- **Class 4**: 951 out of 982 instances were correctly predicted.
- **Class 5**: 861 out of 892 instances were correctly predicted.
- **Class 6**: 933 out of 958 instances were correctly predicted.
- **Class 7**: 1005 out of 1028 instances were correctly predicted.
- **Class 8**: 908 out of 974 instances were correctly predicted.
- **Class 9**: 960 out of 1009 instances were correctly predicted.

**PCA Reduced Dataset**:
- **Class 0**: 967 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1127 out of 1135 instances were correctly predicted.
- **Class 2**: 992 out of 1032 instances were correctly predicted.
- **Class 3**: 988 out of 1010 instances were correctly predicted.
- **Class 4**: 959 out of 982 instances were correctly predicted.
- **Class 5**: 856 out of 892 instances were correctly predicted.
- **Class 6**: 936 out of 958 instances were correctly predicted.
- **Class 7**: 1000 out of 1028 instances were correctly predicted.
- **Class 8**: 922 out of 974 instances were correctly predicted.
- **Class 9**: 968 out of 1009 instances were correctly predicted.

#### Detailed Observations
1. **Higher Correct Prediction Rates**: The PCA Reduced model has higher correct prediction rates across several classes, leading to better overall performance metrics.
2. **Misclassification Trends**: The Block Averaged model shows slightly higher misclassification rates in classes 3, 4, and 8 compared to the PCA Reduced model.
3. **Balanced Performance**: The PCA Reduced model demonstrates a more balanced performance with slightly higher metrics across the board.

#### Conclusion

The neural network model trained on the PCA reduced dataset generally outperforms the model trained on the block averaged dataset. The PCA Reduced model shows higher accuracy, precision, recall, F1 score, balanced accuracy, specificity, and sensitivity. The confusion matrix analysis also indicates that the PCA Reduced model has fewer misclassifications across most classes.

Overall, while both models perform well, the PCA Reduced model is slightly more effective and reliable for the given classification task, demonstrating a more balanced and higher-performing approach.

## 8. ### Conclusions for the Undersampled Dataset Classification Results

#### Performance Metrics
- **Accuracy**: 0.9767 - This indicates that 97.67% of the predictions made by the model are correct, demonstrating high overall performance.
- **Precision**: 0.976535 - High precision indicates a low false positive rate, meaning that when the model predicts a positive class, it is usually correct.
- **Recall**: 0.976690 - High recall indicates that the model correctly identifies a high proportion of actual positives.
- **F1 Score**: 0.976574 - The F1 score, which balances precision and recall, suggests the model has a good balance between these two metrics.
- **Balanced Accuracy**: 0.976690 - Balanced accuracy suggests that the model is equally good at predicting both positive and negative classes.
- **Specificity**: 0.976690 - High specificity indicates that the model correctly identifies a high proportion of actual negatives.
- **Sensitivity**: 0.976690 - Sensitivity, equivalent to recall, shows the model's ability to correctly identify true positives.

#### Confusion Matrix Analysis

The confusion matrix provides a detailed breakdown of actual versus predicted classes:

- **Class 0**: 949 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1117 out of 1135 instances were correctly predicted.
- **Class 2**: 999 out of 1032 instances were correctly predicted.
- **Class 3**: 986 out of 1010 instances were correctly predicted.
- **Class 4**: 968 out of 982 instances were correctly predicted.
- **Class 5**: 877 out of 892 instances were correctly predicted.
- **Class 6**: 940 out of 958 instances were correctly predicted.
- **Class 7**: 1011 out of 1028 instances were correctly predicted.
- **Class 8**: 945 out of 974 instances were correctly predicted.
- **Class 9**: 975 out of 1009 instances were correctly predicted.

#### Error Analysis

- **Class 0**: Very high correct prediction rate with only 31 misclassifications.
- **Class 1**: Few misclassifications, with 18 instances predicted as other classes.
- **Class 2**: Slightly higher misclassifications with instances predicted as classes 3 and 8.
- **Class 3**: Higher misclassification rate with 24 instances predicted as other classes.
- **Class 4**: Some misclassifications into other classes, particularly class 9.
- **Class 5**: Some misclassifications into classes 3 and 0, but overall good performance.
- **Class 6**: Very high correct prediction rate with minimal errors.
- **Class 7**: Some misclassifications into classes 1, 2, and 8.
- **Class 8**: Higher misclassifications into classes 3 and 5.
- **Class 9**: Some misclassifications, but overall high correct prediction rate.

#### Detailed Observations
1. **High Correct Prediction Rates**: Most classes have a high number of correct predictions, demonstrating the model's effectiveness.
2. **Misclassification Patterns**: Misclassifications are generally low and spread across different classes, indicating some areas for improvement.
3. **Class-Specific Observations**: Classes 3, 4, and 8 show relatively higher misclassification rates compared to other classes.

#### Conclusion

The neural network model trained on the undersampled dataset demonstrates high performance across all metrics, with high accuracy, precision, recall, and F1 score. The balanced accuracy suggests that the model treats both positive and negative classes equally well. The confusion matrix reveals a high true positive rate for most classes, indicating strong classification ability.

However, there are some areas for improvement, particularly in classes 3, 4, and 8, where misclassifications are relatively higher. These findings suggest that while the model performs very well, it may benefit from further tuning or additional data to further reduce errors in these specific classes.

Overall, the model is highly effective and reliable for the given classification task, providing strong performance metrics and a balanced approach to class prediction.

## 9. ### Conclusions for the Oversampled Dataset Classification Results

#### Performance Metrics
- **Accuracy**: 0.9130 - This indicates that 91.30% of the predictions made by the model are correct, which is lower compared to other datasets.
- **Precision**: 0.922464 - High precision indicates a low false positive rate, meaning that when the model predicts a positive class, it is usually correct.
- **Recall**: 0.914411 - High recall indicates that the model correctly identifies a high proportion of actual positives.
- **F1 Score**: 0.908214 - The F1 score, which balances precision and recall, suggests the model has a good balance between these two metrics, though it is lower compared to other datasets.
- **Balanced Accuracy**: 0.914411 - Balanced accuracy suggests that the model is equally good at predicting both positive and negative classes.
- **Specificity**: 0.914411 - High specificity indicates that the model correctly identifies a high proportion of actual negatives.
- **Sensitivity**: 0.914411 - Sensitivity, equivalent to recall, shows the model's ability to correctly identify true positives.

#### Confusion Matrix Analysis

The confusion matrix provides a detailed breakdown of actual versus predicted classes:

- **Class 0**: 521 out of 980 instances were correctly predicted, with significant misclassifications into classes 2, 6, and 9.
- **Class 1**: 903 out of 1135 instances were correctly predicted, with notable misclassifications into class 8.
- **Class 2**: 1017 out of 1032 instances were correctly predicted, showing strong performance.
- **Class 3**: 990 out of 1010 instances were correctly predicted.
- **Class 4**: 966 out of 982 instances were correctly predicted.
- **Class 5**: 858 out of 892 instances were correctly predicted.
- **Class 6**: 944 out of 958 instances were correctly predicted.
- **Class 7**: 1001 out of 1028 instances were correctly predicted.
- **Class 8**: 947 out of 974 instances were correctly predicted.
- **Class 9**: 983 out of 1009 instances were correctly predicted.

#### Error Analysis

- **Class 0**: Significant misclassifications, particularly into classes 2, 6, and 9.
- **Class 1**: High misclassifications into class 8.
- **Class 2**: Few misclassifications, demonstrating strong performance.
- **Class 3**: Minimal misclassifications, maintaining high correct prediction rates.
- **Class 4**: Few misclassifications, with most instances correctly identified.
- **Class 5**: Some misclassifications into classes 3 and 0, but overall good performance.
- **Class 6**: Very high correct prediction rate with minimal errors.
- **Class 7**: Some misclassifications into classes 1, 2, and 8.
- **Class 8**: Higher misclassifications into classes 3 and 5.
- **Class 9**: Some misclassifications, but overall high correct prediction rate.

#### Detailed Observations
1. **Lower Overall Accuracy**: The model trained on the oversampled dataset has a lower accuracy (91.30%) compared to other models, indicating it struggles more with the classification task.
2. **High Misclassification Rates**: Significant misclassifications are observed in classes 0 and 1, which impacts the overall performance.
3. **Class-Specific Observations**: Classes 0, 1, and 8 show relatively higher misclassification rates compared to other classes.

#### Conclusion

The neural network model trained on the oversampled dataset demonstrates lower performance across most metrics compared to models trained on other datasets. The accuracy, precision, recall, and F1 score are all lower, indicating the model's reduced effectiveness in this scenario. The confusion matrix reveals significant misclassifications in key classes, particularly class 0 and class 1.

These findings suggest that while the model performs reasonably well, the oversampling approach may have introduced noise or overfitting, reducing its overall generalizability. Further tuning or alternative resampling strategies may be necessary to improve the model's performance on the oversampled dataset.

Overall, the model shows areas for improvement, particularly in reducing misclassifications in classes 0, 1, and 8. These adjustments could help enhance the model's reliability and effectiveness for the given classification task.

## 10. ### Comparison between Oversampled and Undersampled Dataset Classification Results

#### Performance Metrics
| Metric              | Oversampled Dataset | Undersampled Dataset |
|---------------------|---------------------|----------------------|
| Accuracy            | 0.913000            | 0.976700             |
| Precision           | 0.922464            | 0.976535             |
| Recall              | 0.914411            | 0.976690             |
| F1 Score            | 0.908214            | 0.976574             |
| Balanced Accuracy   | 0.914411            | 0.976690             |
| Specificity         | 0.914411            | 0.976690             |
| Sensitivity         | 0.914411            | 0.976690             |

#### Key Observations
1. **Accuracy**:
   - The undersampled model has significantly higher accuracy (0.976700) compared to the oversampled model (0.913000).

2. **Precision**:
   - Precision is higher for the undersampled model (0.976535) compared to the oversampled model (0.922464).

3. **Recall**:
   - Recall is also higher for the undersampled model (0.976690) compared to the oversampled model (0.914411).

4. **F1 Score**:
   - The F1 score, which balances precision and recall, is higher for the undersampled model (0.976574) than for the oversampled model (0.908214).

5. **Balanced Accuracy, Specificity, Sensitivity**:
   - All these metrics are significantly higher for the undersampled model, indicating a more balanced and effective performance in handling both positive and negative classes.

#### Confusion Matrix Analysis

**Oversampled Dataset**:
- **Class 0**: 521 out of 980 instances were correctly predicted, with significant misclassifications into classes 2, 6, and 9.
- **Class 1**: 903 out of 1135 instances were correctly predicted, with notable misclassifications into class 8.
- **Class 2**: 1017 out of 1032 instances were correctly predicted, showing strong performance.
- **Class 3**: 990 out of 1010 instances were correctly predicted.
- **Class 4**: 966 out of 982 instances were correctly predicted.
- **Class 5**: 858 out of 892 instances were correctly predicted.
- **Class 6**: 944 out of 958 instances were correctly predicted.
- **Class 7**: 1001 out of 1028 instances were correctly predicted.
- **Class 8**: 947 out of 974 instances were correctly predicted.
- **Class 9**: 983 out of 1009 instances were correctly predicted.

**Undersampled Dataset**:
- **Class 0**: 949 out of 980 instances were correctly predicted, with minor misclassifications.
- **Class 1**: 1117 out of 1135 instances were correctly predicted.
- **Class 2**: 999 out of 1032 instances were correctly predicted.
- **Class 3**: 986 out of 1010 instances were correctly predicted.
- **Class 4**: 968 out of 982 instances were correctly predicted.
- **Class 5**: 877 out of 892 instances were correctly predicted.
- **Class 6**: 940 out of 958 instances were correctly predicted.
- **Class 7**: 1011 out of 1028 instances were correctly predicted.
- **Class 8**: 945 out of 974 instances were correctly predicted.
- **Class 9**: 975 out of 1009 instances were correctly predicted.

#### Detailed Observations
1. **Higher Correct Prediction Rates**: The undersampled model shows higher correct prediction rates across all classes compared to the oversampled model.
2. **Misclassification Trends**: The oversampled model exhibits significant misclassifications, particularly in classes 0 and 1, whereas the undersampled model has more evenly distributed and fewer misclassifications.
3. **Balanced Performance**: The undersampled model demonstrates a more balanced performance with significantly higher metrics across the board.

#### Conclusion

The neural network model trained on the undersampled dataset significantly outperforms the model trained on the oversampled dataset in terms of accuracy, precision, recall, F1 score, balanced accuracy, specificity, and sensitivity. The confusion matrix analysis indicates that the undersampled model has fewer and more evenly distributed misclassifications, leading to better overall performance.

The oversampled model, while still performing reasonably well, shows higher misclassification rates, particularly in classes 0 and 1, which negatively impacts its overall performance. These findings suggest that the oversampling approach may have introduced noise or overfitting, reducing the model's generalizability.

Overall, the undersampled model is more effective and reliable for the given classification task, demonstrating a more balanced and higher-performing approach compared to the oversampled model.

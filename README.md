# **Customer Purchase Prediction Using K-Nearest Neighbors (KNN)**
This project predicts whether a customer will purchase a product based on their age and estimated salary using the **K-Nearest Neighbors (KNN)** algorithm.

## **📌 Dataset**
- File: `Social_Network_Ads.csv`
- Features: Age, Estimated Salary, Gender (encoded as 0/1)
- Target: `Purchased` (0 = No, 1 = Yes)

## **⚙️ Approach**
- Dropped irrelevant columns (`User ID`), encoded gender.
- Split into train/validation/test sets (60%/20%/20%).
- Feature Scaling using `StandardScaler`.
- Tested K from 1 to 9 to find best accuracy.

## **📊 Results**
- Best K value: **6**
- Final Test Accuracy: **92.50%**
- Precision: 89.19%
- Recall: 94.29%
- F1-Score: 91.67%

## **📈 Classification Report:**
              precision    recall  f1-score   support

     Class 0       0.95      0.91      0.93        45
     Class 1       0.89      0.94      0.92        35

    accuracy                           0.93        80

## **🔁 Cross-Validation**
Performed 10-Fold Cross-Validation on training data.
Average Cross-Validation Accuracy: 87.92%
Shows stable performance across folds and confirms no overfitting.

## **📈 Visualizations**
Confusion Matrix heatmap ,
2D scatter plot showing class separation by age and salary

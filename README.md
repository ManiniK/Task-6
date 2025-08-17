## Task 6: K-Nearest Neighbors (KNN) Classification  

## Objective  
Implement and understand the **K-Nearest Neighbors (KNN)** algorithm for classification using the **Iris dataset**.  

##  Steps Performed  

1. **Data Upload & Inspection**  
   - Uploaded dataset to Colab.  
   - Checked dataset structure, shape, and species distribution.  

2. **Data Preprocessing**  
   - Shuffled dataset to avoid class-order bias.  
   - Dropped unnecessary columns (`Id` if present).  
   - Normalized features using `StandardScaler`.  

3. **Model Training & Validation**  
   - Used `KNeighborsClassifier` from Scikit-learn.  
   - Evaluated model for **K = 1 to 20** using **5-fold cross-validation**.  
   - Plotted Accuracy vs K to find optimal value.  

4. **Model Evaluation**  
   - Selected **best K** based on cross-validation accuracy.  
   - Tested model on hold-out test set (20%).  
   - Evaluated using **Accuracy**, **Confusion Matrix**, and **Classification Report**.  

5. **Visualization**  
   - Confusion matrix plotted as heatmap.  
   - Decision boundary visualized using **first two features** (Sepal Length & Sepal Width).  


## Results  

- **Best K**: 7 (based on cross-validation).  
- **Test Accuracy**: ~0.9 (depending on split).  
- Confusion matrix shows very few misclassifications.  
- Decision boundary shows clear separation between classes in feature space.  

## Observations  
- KNN works very well on the Iris dataset due to clear class separability.  
- Feature scaling is **essential** for distance-based models.  
- Very small K can lead to overfitting, while larger K smooths decision boundaries.  
- Using all 4 features gives near-perfect accuracy.  


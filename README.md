# 2nd Phase of CIS Trainee Program  
This project is part of the Trainee process of the IEEE Computational Intelligence Society (CIS) Student Chapter at the University of Brasília (UnB): Week 2.  
**Student**: Vinicius Nascimento  

## a) "Binary classification to predict if a wine is red or not":  
The assigned dataset was "Wine Quality," available at this [link](https://drive.google.com/file/d/14Y6ZJYI-sB_T9tHexlg2GCSfLCmC6eQE/view). I used the KNN (K-Nearest Neighbors) method to determine if a wine was red based on binary classification. The reference column was `Wine_Is_Red`, which is the last column of the dataset. Using the KNN method from the Python SKLearn library, I achieved an accuracy of 93% with an 80%-training and 20%-testing dataset split.

## b) "Multiclass classification to predict wine quality":  
To predict wine quality, I noted that some authors from reference sources suggested generating a correlation matrix of the data. After generating the matrix, I identified the factors most correlated with wine quality (the last column). The parameter mapping was done using a Column Number-Name relationship.  

Next, I applied the Random Forest algorithm to meet the requirements and proceed to item d.

## d) "Feature Importance - Apply the Random Forest algorithm and determine which features in the dataset are most important for the problem":  
After achieving an accuracy of 68%, I concluded that the model was insufficient for reliable prediction. I extracted the confusion matrix to verify which classes were predicted most accurately. The analysis showed that class 3 wines were the most accurately predicted.  

Subsequently, I generated the feature importance output as requested.

## e) "Apply data normalization and evaluate the effects on the models":  
I normalized the dataset and observed that the KNN model achieved an accuracy of 58.15%, while the Random Forest model achieved 69%. Additionally, I noticed from reference sources that the number of wines for each quality class was imbalanced, with more wines in classes 6, 5, and 7, respectively. I later understood the importance of dataset balancing, as discussed in item f.

## f) "Apply undersampling and oversampling techniques to the dataset. Evaluate and explain the effects":  
- _"Oversampling: This technique artificially increases the number of instances in the minority class to balance class proportions. This is typically done by replicating existing samples or generating new synthetic instances based on the current minority class samples."_  
- _"Undersampling: This technique reduces the number of instances in the majority class to balance it with the minority class. It is performed by randomly or strategically selecting a subset of the majority class samples."_  

Since the samples at the edges of the quality level frequency distribution were significantly smaller than the values for classes 5, 6, and 7, I opted to use oversampling as it was more appropriate for the dataset. For this, I utilized the `imblearn` library, which provides sampling methods via import.

## g) "Apply one of the Ensemble Learning methods and compare the results":  
- _"Ensemble Learning refers to a machine learning approach where multiple models are combined to perform a predictive or classification task. Instead of relying on a single model, ensemble learning leverages the collective wisdom of several models to enhance overall accuracy and system performance."_  

## h) "Implement a KNN using only NumPy":  
This was completed without using the Pandas library. However, I found that Pandas would have been helpful for plotting boxplot graphs and identifying outliers in some features deemed important for wine quality, as indicated by the correlation matrix.

### Observations:  
The following concepts and techniques were applied:  
- KNN (K-Nearest Neighbors)  
- Support Vector Machine  
- Decision Tree  
- Random Forest  
- Binary Classification  
- Multiclass Classification  
- Evaluation Metrics (Cross-validation, Confusion Matrix, Precision, and Recall)  
- Ensemble Learning  
- Data cleaning and manipulation  
```
![thinkstockphotos-615269202](https://github.com/ViniciusGN/CIS-2-Trainee/assets/80403948/6cdd6189-8eba-416f-81ba-56f68b9633d6)

### Curiosidade: 
Você sabia que acredita-se que as vinhas mais antigas do mundo estão localizadas na região da Cachemira, no norte da Índia?

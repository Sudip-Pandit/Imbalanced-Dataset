# Imbalanced-Dataset

# Introduction 


A datset which consists classes having large number data in one class and less number of data in other class, called imbalanced dataset. The machine learning model which is builded by the imbalanced dataset might be predicting the class having large dataset but works very poor on the class which has less dataset as compared to the large dataset. Though, model accuracy would be too high but it does not work for the target class which has less data. 
The credit card fraud detection is one example of that imbalanced dataset. The credit card fraud detection machine learning model suffered badly due to the imbalanced dataset issue. It has very less fraud transcation than non-fraudulent transcations. The fraud transaction cases are very few. The other examples are manufacturing defect, rare disease diagnosis etc. We heard many fraud detection machine learning model has not been predicting the fraudulent cases and similarly, the deadly disease diagnosis prediction has also been less accuracy. 

# Problem statement


The imbalanced dataset is challenging  for the machine learning model. We develop baseline model and comparing. we develop baseline model at first and the successive machine learning models. We expect successive machine learning model's accuracies and classification metrics should have some distinct results (metrices should have good results than the baseline model). But, due to the heavily imbalanced dataset, the machine learning model predicts good results on class having large number of datasets than class having less number of dataset.  Thus, it is very important to balance the dataset before proceeding  machine learning model. This project finds the best way to balance the imbalanced dataset.
What is the technique to balance the imbalanced dataset? what are the different methods to deal with imbalanced dataset? How do we know the imbalanced dataset?


# Problem analysis

+ I analyze the imbalanced dataset with help of sklearn library. I will run command pip install imbalanced-learn and then import import imblearn.  
+ We have different techniques to balance the dataset such as upsampling (random over-sampling) the small number of dataset, dowmsampling (random under-sampling) of large number of dataset and make balance. The smote technique is very popular in balancing the imbalanced dataset. 
+ The following are the steps used in smote technique:
      + First we identify the feature vector and its nearest neighbour
      + The next step is to take the difference between two feature vectors
      + The difference should multipy with a random number between 0 and 1
      + Find a new point on the line between the two vectors and adding the random number to feature vector
      + The process should repeat on the others feature vectors
      + Finally, create new "synthetic" observations




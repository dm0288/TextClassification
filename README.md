# TextClassification

This repo contains ipython notebook that implements different classifier for the text classification.

## Method

### Importing Libraries:

First of all we need to import all the required libraries

### Importing Data:

The given data file is loaded using pandas read_csv and both the columns has been given the name as desc and label .

### Data Preparation:

Now the text needs to be preprocessed before proceeding further. Text may contain numbers, special characters, unwanted spaces and stopwords. And here in this problem, we don't need the presence of all these. These will unnecessarily add confusion and complexity. Hence, we will remove all the special characters, unwanted spaces and stop words from our text. 

Also the data is divided to train and test set.

### Feature Engineering:

Raw text data needs to be transformed into feature vectors. The following methods will be applied to obtain relevant features from our dataset.
- Count Vectors features
- TF-IDF Vectors features
    - Word level
    - N-Gram level 
    - Character level
        
### Modle Building:

The final step in the text classification framework is to train a classifier using the features created. There are many different machine learning models which can be used to train a model to classify text. We will implement following different baseline classifiers for this purpose;
- Naive Bayes Classifier (Has been proved to be very effective for text classification with small and simple dataset)
- Logistic Regression (Works well with small dataset which is linearly separable. Data with very high dimensions tend to be linearly separable. Hence it works pretty welll with text data)
- Random Forest (Handles high dimensional and sparse data well)
- Extreme Gradient Boost (Popular, fast and accurate. Used for the purpose of comparison)
    
 ## How to run
 - Download the repository. It contains the input data file and required trained model files along with the source code.
 
 - ```cd source/```
 - ```jupyter notebook```  (This launches the jupyter notebook)
 - Now open the TextClassification.ipynb file and click on run all. This shows the performance of test set on different type feature and model. At the end it asks to enetr a text for classification. 

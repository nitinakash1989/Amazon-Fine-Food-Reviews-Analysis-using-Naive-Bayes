
# Amazon Fine Food Reviews Analysis using Naive Bayes

## Objective


Given a review determine polarity of the review( Polarity: Whether a review is positive or negative)

<i><b>How to determine polarity of the review?</b></i>

We can use score column from the amazon dataset to determine whether a review is positive or negative.

- Score(4 and 5) --> Positive review
- Score(1 and 2) --> Negative review
- Score 3 --> Nutral


<b>Data Source</b>: https://www.kaggle.com/snap/amazon-fine-food-reviews <br>

# Steps

The ipython notebook consist of below steps.
- Reading data: The data source is present in two format but we used sqllite because it will be easy for us to query the database

- Data Profiling: To find the basic statistics of the data.
- Data Cleaning: This is one of the crucial step in the analysis. We performed below operation to clean the data so that it will be ready for preprocessing.
    1. Mapping of review score to polarity
    2. Converting text to lowercase
    3. Converting Time to datetime format
    4. Deduplication
    5. Rule based filtering
    6. Sampling and balancing the dataset

- Data Preprocessing: After cleaning of data we preprocessed the data by following below steps.
    1. Remove stopwords
    2. Remove punctuations.
    3. HTML tag removal
- Split Data into train, validate and test dataset.
- Feature Engineering: After the data is cleaned and ready to process, we did featurization to convert text to vector. For this , I follow below algorithms
    1. Bag Of Words (BoW)
    2. Term Frequency - inverse document frequency (tf-idf)
- Note: We can't use Word2Vec with Naive Bayes because it W2V generated vector with -ve values. 
- Model Fitting and testing: For all the dataset genererated in feature engineering, we fit the model and did the testing to find accuracy of the model.


- Ploting ROC curve
- <a href="https://www.kaggle.com/nitinakash1989/amazon-fine-food-reviews-analysis-using-knn">KNN</a> vs <a href="https://www.kaggle.com/nitinakash1989/amazon-fine-food-review-analysis-using-naive-bayes">Naive Bayes</a>


```python

```

<i><b><font color="green">Notebook in Kaggle:  --></font></b></i><a href = "https://www.kaggle.com/nitinakash1989/amazon-fine-food-review-analysis-using-naive-bayes">Download</a>

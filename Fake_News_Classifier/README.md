# 1. Project Summary 
This project studies text classification of misinformation with PySpark. 
As humans we understand (at least sometimes) what news is fake and what news is true because our minds have a representation of the real world. Computers do not have this representation to determine fake news. This begs the question: Can factual news be distinguished from fake news by a machine learning model based purely on the words in a text and their frequency?
To address this question using a standard NLP workflow, this project:
1) Loads data of fake and true news from [Kaggle](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset?select=Fake.csv)
2) Cleans the data
3) Preprocesses the text documents (Tokenize and remove stop words)
4) Performs feature vectorization (CountVectorizer and IDF)
5) Fits a model (Logistic Regression)
6) Evaluates results (AreaUnderROC, Accuracy, Confusion Matrix)

I find that the logistic regression model performs with **91% accuracy** on this task. Examining the specific coefficients of individual tokens does not reveal clear distinctions in the kinds of words used in fake versus true news. Therefore, future analysis is recommended to determine how generalizable this particular model would be for novel datasets.


# 2. Table of Contents
    a. presentation.pdf
        - slides for final presentation to DATA603 class
    b. misinfo_classification_data603-final-project.ipynb  
        - jupyter notebook of EDA, modeling, and results with outputs

# 3. Guide on Running Code
To run the notebook corresponding to this project, installing Spark and all related dependencies (e.g., Java driver, etc.) is necessary. In the creation of the SparkSession, this notebook defines several Spark configurations dealing with driver and executor memory. The values assigned to these configs should correspond to your local machine's memory capacity. These configs are included to account for persistent errors relating to Java-side processes that occurred when running without them on the entire original dataset. 
Once all dependencies are set up, the notebook can be run through a docker container. The one used in development is accessible using the `docker pull jupyter/pyspark-notebook` in the command line. 
Running the code will also require you to download the two files from the Kaggle link above. Keep the file names unchanged and place them in the same location as the notebook.

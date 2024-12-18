# Goodreads-Review-Rating

# Description
In this project we predicted the numerical rating associated using solely the review's text content.  

# Dataset
We used the GoodReads review dataset from Kaggle: https://www.kaggle.com/datasets/pypiahmad/goodreads-book-reviews1?select=goodreads_reviews_dedup.json 

# File Descriptions
LSTM.ipynb - Our final project file with our LSTM model structure. 

DataPreprocessing.ipynb - The file that loads, cleans, and preprocesses the data creating DistilBERT embeddings. 

Linear_Regression.ipynb - The baseline Linear Regression model we created. 

GRU.ipynb - The baseline GRU model we created. 

EDA.ipynb - The initial exploratory data analysis.

sample_experiments_Word2Vec.ipynb - Some sample experiments with Word2Vec purely for example purposes. Not very cleaned. 

# Instructions
For running LSTM.ipynb, please add the following file to your drive: 

https://drive.google.com/file/d/1gu1LkiRNbcojJCkeJBOEci8q3edpz3uA/view?usp=drive_link

That is the DistilBERT embeddings for 300k data instances. You can then open the notebook in Colab and run the code. Alternatively, you may open the notebooks in Jupyter, in which case you would have to download the pkl file, edit the first few code cells to access the file from your local device, after which the rest of the code would remain the same. 

For running any of the files beside LSTM.ipynb, please download the goodreads_reviews_dedup.json from the above Kaggle link. Then unzip the file and upload it to your Google Drive. You can then open the notebooks in Colab and run the code. Alternatively, you may open the notebooks in Jupyter, in which case you would have to edit the first few code cells to unzip the file from your local device, after which the rest of the code would remain the same. 

# Framework


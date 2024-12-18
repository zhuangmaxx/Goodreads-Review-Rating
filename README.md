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

<img width="371" alt="image" src="https://github.com/user-attachments/assets/16ed096e-11b0-490f-8ff6-76e6c9961816" />

<img width="351" alt="image" src="https://github.com/user-attachments/assets/40a93d55-8f3d-43d4-824a-9a03dc4aa457" />


# Results

<img width="431" alt="image" src="https://github.com/user-attachments/assets/39ea7c47-9388-4317-b0ba-f21478996ad3" />

<img width="413" alt="image" src="https://github.com/user-attachments/assets/5c81d48b-3d6e-4e82-82a0-5e2ed5c9b66e" />

# References

[1] Joshua Phuong Le. (2022, August 17). Rating Prediction from Review Text with
Regularization — Linear Regression vs Logistic Regression. Medium; MITB For All. https://medium.com/mitb-for-all/ rating-prediction-from-review-text-with-regularization-linear-regression-vs-logistic-regression-df0181fe9c0

[2] Asterios Bampakis et al. (2020). Products review rating prediction from users’ text reviews. GitHub. https://github.com/stergiosbamp/nlp-review-rating-prediction/ blob/main/paper/Products-review-rating-prediction-from-users-text-reviews.pdf

[3] Ahmed, B. H., & Ghabayen, A. S. (2020). Review rating prediction framework using deep learning. Journal of Ambient Intelligence and Humanized Computing, 13(7), 3423–3432. https://doi.org/10.1007/s12652-020-01807-4

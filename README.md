# Goodreads-Review-Rating

# Description
We want to predict the numerical rating associated with a review based on its text
content. For this we will be using the GoodReads review dataset which has the X reviews
with some associated metadata such as user and book IDs, and of course the numerical
rating as a number between 1 and 5 inclusive. Our project aims to see if it is possible to
reasonably and accurately make these predictions utilizing a neural network. 

Milestone 1: https://files.campuswire.com/7d5dc920-2dc5-444d-a8ab-c63f835fb5f7/5281cd94-27c1-40e8-b2a3-992dccc23c0d/Numerical%20Rating%20Prediction%20from%20Goodreads%20Text%20Reviews.pdf

# Contents

# References
https://github.com/AGiannoutsos/Twitter-Sentiment-Analysis-with-LSTMs-ELMo/tree/main 

https://www.kaggle.com/code/athoul01/predicting-yelp-ratings-from-review-text

https://machinelearningmastery.com/combine-oversampling-and-undersampling-for-imbalanced-classification/#:~:text=Manually%20Combine%20SMOTE%20and%20Random%20Undersampling,-We%20are%20not&text=The%20authors%20of%20the%20technique,better%20than%20plain%20under%2Dsampling.

# Improvements
For this milestone work on preprocessing and embeddings 

1. **Data Preprocessing**:
   - **Text Cleaning**: Standardize text preprocessing. Consider removing special characters, URLs, and extra whitespace, and convert text to lowercase to reduce vocabulary size.
   - **Stopwords and Lemmatization**: Your notebook imports `WordNetLemmatizer` and `stopwords` from NLTK, but make sure they are applied to reduce noise further.
   - **Sentence Tokenization**: If reviews are long, sentence-level tokenization can improve LSTM performance by creating shorter, more meaningful sequences.

2. **Embedding Layer**:
   - **Pre-trained Embeddings**: Replace Keras’s Embedding layer with pre-trained embeddings like GloVe or FastText to provide your model with richer semantic information, reducing the need for the model to learn basic word relationships from scratch.
   - **Trainable Embedding Layer**: If pre-trained embeddings are not feasible, ensure your embedding layer is trainable to allow it to adapt to the specific vocabulary and context of the reviews.

3. **Model Architecture**:
   - **Stacked LSTM Layers**: Add an additional LSTM layer if the data complexity justifies it. Stacking LSTM layers often captures more complex patterns in text data.
   - **Bidirectional LSTM**: Bidirectional LSTMs improve context understanding by reading sequences both forward and backward, which is beneficial for text with complex structures.
   - **Dropout Regularization**: Increase dropout in LSTM layers to prevent overfitting, particularly if your dataset is large.

4. **Hyperparameter Tuning**:
   - Experiment with the following:
     - **Sequence Length**: Adjust `max_length` in `pad_sequences` based on the typical review length to capture enough context without adding unnecessary padding.
     - **Batch Size**: Test different batch sizes (e.g., 32, 64, 128) for an optimal balance between training stability and speed.
     - **Learning Rate**: Tune the learning rate and consider using a learning rate scheduler or cyclical learning rate to improve convergence.

5. **Training Process**:
   - **Early Stopping and Checkpointing**: Use early stopping based on validation loss and save the best-performing model with checkpointing.
   - **Cross-Validation**: Perform k-fold cross-validation if the dataset size allows to ensure the model generalizes well.

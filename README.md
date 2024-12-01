# Movie Genre Classification from Descriptions

## Objective

The goal of this project is to classify movies into their respective genres based on the description of the movie. The classification is performed using Natural Language Processing (NLP) techniques for feature extraction and classification algorithms to predict the movie genre.

---

## Dataset

The dataset used in this project is available on Kaggle:  
[Kaggle Dataset Link](https://www.kaggle.com/datasets/hijest/genre-classification-dataset-imdb)

---

## Steps Taken

### 1. Data Preprocessing
- **Text Preprocessing:** Applied NLP techniques to prepare the data for modeling:
  - **Stopwords Removal:** Removed common words that do not contribute much to the meaning.
  - **Tokenization:** Split movie descriptions into words or tokens.
  - **Lemmatization:** Reduced words to their base or root form to standardize the text.

### 2. Feature Extraction
- **TF-IDF (Term Frequency-Inverse Document Frequency):** Transformed the text into numerical vectors based on word importance across the corpus.
- **Word2Vec:** Used Word2Vec embeddings to represent words in the descriptions as vectors, capturing the semantic meaning of words.

### 3. Model Building
- **Logistic Regression:** Trained a logistic regression model using the extracted features (both TF-IDF and Word2Vec).
- **Naive Bayes:** Also trained a Naive Bayes model to compare performance.

### 4. Model Evaluation
- **Comparison:** Inferred that the Logistic Regression model outperformed Naive Bayes. Additionally, TF-IDF embeddings provided better results than Word2Vec.

---

## Kaggle Notebook

You can find the complete code implementation and analysis in my Kaggle notebook:  
[Kaggle Notebook Link](https://www.kaggle.com/code/varshithpsingh/movie-genre-classification)

---

## Insights and Results

- Logistic Regression performed better than Naive Bayes for movie genre classification.
- TF-IDF embeddings were more effective in capturing important features from the movie descriptions compared to Word2Vec embeddings.
- The final model successfully predicted the movie genres, providing a basis for further improvements in text classification tasks.

# Sentiment Analysis on Tweets

## Overview

This project performs **sentiment analysis** on a collection of tweets using traditional machine learning classifiers. The goal is to classify each tweet as **positive**, **negative**, or **neutral** based on its content. This solution demonstrates that robust results can be achieved even without deep learning, using proper preprocessing and classical ML techniques.

---

## Technologies Used

- Python 3.11.4
- Jupyter Notebook
- Pandas, NumPy
- Scikit-learn - for text vectrization and model building and pipelining
- gensim - to use google pretrained word2vec

---

## Project Structure

- `train.csv` : training data
- `test_pred.csv` : valuation_data
- `sentiment_analysis.ipynb` : scripts

---

## Workflow

1. **basic Preprocessing**  
   - Lowercasing  
   - Removing punctuation, stopwords, URLs, mentions  
    

3. **Feature Extraction**  
   - TF-IDF Vectorization  

3. **Data Preparation**
   - Along With TF-IDF vectorization, incoperated google word2vec pretrained data using gensim
   - Creating a average sentence vector using pretrained word2vec weighted by rarity of the word using tf_idf

4. **Modeling**  
  - trained three separate model based on 
  1. full_model3 - Pipeline consisting LogisticReggression on TF-IDF vectorized text
  2. full_model2 - Pipeline of TF-IDF without stop words and naive_bayes MultinomialNB
  3. full_model1 - Pipeline of prepared data with gensim and LogisticReggression
  4. final_model - The best two full_model1 and full_model3 were used on a voting classifier in order to account both the training
                   data and the global pretrained word2vec data
  

5. **Evaluation Metrics**  
   - Precision, Recall
   - Confusion Matrix  

---

## Results

*(Update this section with your actual metrics)*

| Classifier           | Precision | Recall |
|----------------------|-----------|--------|
| full_model3          | 0.76      | 0.76   |
| full_model2          | 0.66      | 0.66   |
| full_model1          | 0.75      | 0.75   |
| final_model          | 0.82      | 0.82   |

---


## Conclusion

This project shows that even without deep learning, a well-processed pipeline with classical machine learning can yield nice results for sentiment analysis.

---

## Future Enhancement

- Using deep learning models like LSTM
- Trying out different models and ensemble methods


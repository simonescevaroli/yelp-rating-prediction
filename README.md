Project for _Natural Language Processing_ (_Politecnico di Milano_, 2023-2024)

# Natural Language Processing
This repository contains the main notebook created for the Natural Language Processing (NLP) course project.<br>
The notebook was executed on Kaggle using a GPU P100. To test the notebook, you will need to download the "sentiment-analysis-word-lists-dataset".

## Rating prediction and sentiment analysis
The primary tasks of this project were to perform star rating prediction and sentiment analysis on a large collection of product reviews.<br>
The notebook explores various approaches and models. The following steps were undertaken:
1. **Initial Data Analysis**: Conducted an initial analysis to understand the dataset's composition.
2. **Word Embeddings**: Utilized embeddings to examine the geometric properties of the words in the dataset.
3. **Clustering Techniques**: Experimented with different clustering techniques.
4. **Model Exploration**: Evaluated a wide variety of models, including linear classifiers, random forest classifiers, LSTMs, and Transformers.
5. **Sentiment Analysis**: Performed sentiment analysis on the reviews.
6. **Cross-Dataset Evaluation**: Conducted rating prediction and sentiment analysis on a different dataset to assess the performance of pre-trained models.

## Datasets
The main dataset used for the project was the YELP review dataset [YELP dataset](https://huggingface.co/datasets/yelp_review_full), containing 700k reviews with text and star ratings (1 to 5 stars).<br>
An additional dataset from Amazon containing reviews of electronic products [Amazon dataset](https://huggingface.co/datasets/rkf2778/amazon_reviews_mobile_electronics), comprising 100k reviews, was also utilized.

## Results
As expected, the highest results were achieved using Transformers, which are the current state-of-the-art for classification tasks.

- **Rating Prediction**: Achieved an F1 score of 0.71 using the XLNet model. XLNet is an extension of the Transformer-XL model pre-trained using an autoregressive method to learn bidirectional contexts by maximizing the expected likelihood over all permutations of the input sequence factorization order.
- **Sentiment Analysis**: Achieved an F1 score of 0.9 using the DistilBERT model.

## Team
Andrea Alari, Francesco Barisani, Elisa Composta, **Simone Scevaroli**

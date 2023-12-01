# Influencer Style Language Model

## Overview

This project aims to create a language model that generates text in the style of a selected influencer. It involves data gathering from social media, data processing, sentiment analysis, and fine-tuning a GPT-2 language model. Users can then interact with the model through a simple interface.

## Requirements

1. **Python 3.x**
2. Required libraries: tweepy, pandas, numpy, re, nltk, textblob, matplotlib, seaborn, gpt_2_simple, wordcloud
3. API keys for Twitter (if using the Twitter API)

## Instructions

### Data Gathering

1. If using Twitter:
   - Set up Twitter API credentials.
   - Specify the target influencer's username.
   - Collect tweets from the target user using `tweepy`.

### Data Processing

1. Load the raw data from the CSV file (`rawdata.csv`).
2. Clean the tweets by removing retweets, hashtags, hyperlinks, mentions, and emojis.
3. Perform sentiment analysis using TextBlob.
4. Visualize the data with scatter plots, histograms, and word clouds.

### Model Fine-Tuning

1. Download the GPT-2 model (124M) using `gpt_2_simple`.
2. Save the cleaned tweets as a text file (`tweet.txt`).
3. Start a TensorFlow session and fine-tune the GPT-2 model using the `gpt2.finetune` function.

### Interface Development

1. Develop a simple interface where users can input responses.
2. Use the fine-tuned GPT-2 model to generate influencer-style posts based on user inputs.

### Testing and Evaluation

1. Test the model's outputs for quality, relevance, and similarity to the original posts.
2. Implement a testing framework and obtain user feedback for evaluation.

## Code Structure

1. `data_processing.ipynb`: Jupyter notebook for data processing.
2. `sentiment_analysis.ipynb`: Jupyter notebook for sentiment analysis.
3. `gpt2_finetuning.ipynb`: Jupyter notebook for GPT-2 fine-tuning.
4. `interface.py`: Python script for the user interface.
5. `testing_evaluation.ipynb`: Jupyter notebook for testing and evaluation.

## Important Notes

- Ensure compliance with ethical guidelines and terms of service when gathering data from social media platforms.
- Adjust fine-tuning parameters based on available resources and training requirements.

## Future Improvements

- Consider incorporating user feedback for iterative model improvement.
- Explore more advanced fine-tuning techniques and larger GPT-2 models for improved performance.

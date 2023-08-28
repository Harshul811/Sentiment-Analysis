# Sentiment Analysis Project

This project involves analyzing the sentiment of text data using Natural Language Processing (NLP) techniques. The provided Python script reads text data from a file, processes it, performs sentiment analysis, and visualizes the emotions detected. This document provides an overview of the project, the script's functionality, and how to use it.

## Table of Contents

- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Usage](#usage)
- [Script Explanation](#script-explanation)
  - [Text Preprocessing](#text-preprocessing)
  - [Emotion Analysis](#emotion-analysis)
  - [Sentiment Analysis](#sentiment-analysis)
  - [Emotion Visualization](#emotion-visualization)
- [Conclusion](#conclusion)

## Project Overview

The project demonstrates sentiment analysis on text data using Python and NLP techniques. It processes a text document, identifies emotions associated with specific words, performs sentiment analysis, and visualizes the emotions detected in the text.

## Getting Started

### Prerequisites

- Ensure you have Python installed on your system.
- Install required NLTK dependencies using: `pip install nltk`
- Download the NLTK stopwords corpus using: `nltk.download('stopwords')`
- Download the NLTK punkt tokenizer using: `nltk.download('punkt')`
- Download the NLTK VADER sentiment analyzer using: `nltk.download('vader_lexicon')`
- Place the `read.txt` file containing the text data in the same directory as the script.
- Create an `emotions.txt` file containing emotion-word associations, one per line: `word: emotion`

### Usage

1. Clone or download the repository.

2. Open a terminal or command prompt and navigate to the project directory.

3. Run the script: `python sentiment_analysis_script.py`

4. The script will process the text data, perform sentiment analysis, and generate a sentiment analysis result along with an emotion visualization graph.

## Script Explanation

### Text Preprocessing

- The script reads text data from `read.txt`.
- Converts the text to lowercase and removes punctuation.
- Tokenizes the text using the NLTK tokenizer.
- Removes stopwords from the tokenized words.
- Performs lemmatization on the remaining words.

### Emotion Analysis

- The script reads emotion-word associations from `emotions.txt`.
- For each word in the processed text, if the word is found in the emotion associations, the corresponding emotion is recorded.

### Sentiment Analysis

- The script utilizes the VADER sentiment analyzer from NLTK to perform sentiment analysis on the entire text.
- It determines whether the sentiment is positive, negative, or neutral.

### Emotion Visualization

- The script generates a bar graph depicting the count of emotions detected in the text.
- Saves the visualization as `graph.png`.

## Conclusion

This Sentiment Analysis project showcases how to process text data, analyze emotions associated with words, perform sentiment analysis, and visualize emotions using Python and NLP techniques. The provided script, `sentiment_analysis_script.py`, serves as an example of how to accomplish these tasks.


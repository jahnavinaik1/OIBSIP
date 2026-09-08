
# Autocomplete and Autocorrect System

## Project Overview

This project implements a basic Natural Language Processing (NLP) based system for **autocomplete and autocorrect** functionality. The system analyzes a text corpus to identify frequently occurring words, generate next-word suggestions, and provide possible corrections for misspelled words.

The project demonstrates fundamental NLP techniques that can be applied to intelligent text input and language assistance systems.

## Objectives

The primary objectives of this project are:

* To analyze and preprocess textual data.
* To perform word frequency analysis.
* To develop a bigram-based autocomplete model.
* To generate next-word suggestions for a given input.
* To implement an autocorrect mechanism using word similarity.
* To develop an interactive text assistant combining autocomplete and autocorrect functionality.

## Dataset

The project uses the **Gutenberg Corpus** provided by the Natural Language Toolkit (NLTK).

**Source Text:** *Emma* by Jane Austen

The corpus is used as the training text for analyzing word occurrences and relationships between consecutive words.

## Technologies and Libraries

The project was developed using Python and the following libraries:

* **Python**
* **NLTK** – Natural Language Processing and corpus processing
* **Pandas** – Data handling and result management
* **Matplotlib** – Data visualization
* **Collections** – Word frequency and bigram analysis
* **Difflib** – Similarity-based autocorrect suggestions

## Methodology

### 1. Text Preprocessing

The text from the Gutenberg corpus is loaded and processed to prepare it for analysis. The text is converted to lowercase and non-alphabetic tokens are removed.

### 2. Word Frequency Analysis

The frequency of individual words is calculated using Python's `Counter`. This helps identify the most frequently occurring words in the corpus.

### 3. Bigram Model

A bigram model is constructed by analyzing pairs of consecutive words. The model records which words commonly follow a particular word.

For example:

```text
Input Word → Possible Next Words
```

The most frequently occurring next words are used as autocomplete suggestions.

### 4. Autocomplete

The autocomplete functionality accepts a word or sentence and generates possible next-word suggestions based on the bigram model.

### 5. Autocorrect

The autocorrect functionality compares an unknown or misspelled word with words present in the corpus. Similar words are identified using Python's `difflib` module.

### 6. Smart Text Assistant

The autocomplete and autocorrect components are combined into a single text assistant. The system determines whether the entered word is present in the vocabulary and provides either next-word suggestions or possible corrections.

## Project Structure

```text
DataAnalytics-L1-Autocomplete-Autocorrect/
│
├── Autocomplete_Autocorrect.ipynb
├── autocomplete_autocorrect_results.csv
├── README.md
│
└── screenshots/
    ├── word_frequency.png
    ├── autocomplete_result.png
    └── autocorrect_result.png
```

## Results

The implemented system successfully performs the following tasks:

* Identifies frequently occurring words in the corpus.
* Generates next-word suggestions using a bigram model.
* Provides autocomplete suggestions for sentence input.
* Identifies possible corrections for misspelled words.
* Combines autocomplete and autocorrect into an interactive text assistant.

The generated results and visualizations are included in the `screenshots` directory.

## Key Learning Outcomes

Through this project, the following concepts were explored:

* Natural Language Processing fundamentals
* Text preprocessing
* Word frequency analysis
* N-gram language modeling
* Bigram-based prediction
* String similarity and autocorrection
* Data visualization using Matplotlib
* Python-based text processing

## Conclusion

This project demonstrates a fundamental implementation of autocomplete and autocorrect using Natural Language Processing techniques. The combination of word frequency analysis, bigram modeling, and similarity-based matching provides a simple approach to intelligent text prediction and correction.

The project serves as an introductory implementation of NLP concepts and provides a foundation for developing more advanced language-processing applications.

## Author

**Jahnavi Naik**

Bachelor of Engineering
Computer Science and Business System
Canara Engineering College


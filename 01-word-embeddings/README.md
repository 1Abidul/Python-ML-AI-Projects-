# Exploring Word Embeddings in Python

**Assignment 1** · Abidul Hasib · September 2026

A hands-on look at **word embeddings**: how a model represents each word as a list of numbers so that words with similar meanings sit close together.

## What I did
1. **Loaded a pre-trained model:** GloVe `glove-wiki-gigaword-50`, through `gensim.downloader`.
2. **Inspected a word vector:** the word *ocean* is represented by **50 numbers**, one per dimension, learned from how the word is used in large amounts of text.
3. **Compared word similarities** using cosine similarity.
4. **Found the most similar words** to *school*, *music* and *doctor*.

## Results

### Word similarity

| Word 1 | Word 2 | Similarity |
|---|---|---|
| cat | dog | **0.9218** |
| coffee | tea | 0.8080 |
| doctor | nurse | 0.7977 |
| king | queen | 0.7839 |
| cat | computer | 0.3525 |
| river | banana | 0.2823 |

Related pairs (pets, drinks, professions, royal titles) score high, while unrelated pairs score low.

### Most similar words

| Word | Top 5 nearest words |
|---|---|
| school | college (0.93), schools, campus, graduate, elementary |
| music | musical (0.89), pop, dance, songs, recording |
| doctor | nurse (0.80), physician, patient, child, teacher |

## Key takeaway
The model learns meaning from **context**: words used in similar sentences get similar vectors. That's why *doctor* ends up near *teacher* and *child*. They aren't synonyms, but they often appear in the same kinds of text.

## How to run
Open `Exploring_Word_Embeddings_in_Python.ipynb` in Google Colab or Jupyter and run the cells in order. The first cell installs Gensim, and the model (about 66 MB) downloads automatically.

**Tools:** Python, Gensim, GloVe

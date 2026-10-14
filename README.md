# Python ML & AI Projects

A collection of my school projects and assignments in **Python, machine learning and artificial intelligence**. Each project is in its own folder with its notebook or code and a short README explaining what it does and what I found.

**Author:** Abidul Hasib

---

## Projects

| # | Project | Topic | Tools | Folder |
|---|---|---|---|---|
| 1 | **Exploring Word Embeddings in Python** | NLP: how words are turned into vectors and compared by meaning | Python, Gensim, GloVe | [`01-word-embeddings/`](01-word-embeddings/) |

*More projects will be added as I complete them.*

---

## Project summaries

### 1. Exploring Word Embeddings in Python
Uses a pre-trained **GloVe** model (`glove-wiki-gigaword-50`, loaded with Gensim) to explore how a computer represents the meaning of words.
- Inspects a word's **50-dimensional vector** ("ocean").
- Compares words with **cosine similarity**: *cat–dog* scores **0.92**, *king–queen* **0.78**, and *cat–computer* only **0.35**.
- Finds each word's **nearest neighbours**: the closest words to *school* are *college*, *schools*, *campus*, *graduate* and *elementary*.
- Explains why some neighbours are surprising: *doctor* lands close to *teacher* and *child* because those words appear in similar sentences.

[View the notebook →](01-word-embeddings/Exploring_Word_Embeddings_in_Python.ipynb)

---

## Repository structure

```
Python-ML-AI-Projects-/
├── 01-word-embeddings/
│   ├── Exploring_Word_Embeddings_in_Python.ipynb
│   └── README.md
└── README.md
```

## Running the notebooks
Each notebook runs in **Google Colab** or **Jupyter**. Packages are installed in the first cells (for example `!pip install gensim`).

## Skills
Python · Jupyter / Google Colab · Natural language processing · Word embeddings (GloVe) · Gensim

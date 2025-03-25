# Occupation or Self-Defence?
### A Computational Analysis of NYT Framing, U.S. Foreign Policy, and Public Opinion during the Israel-Hamas War (Oct 2023–Oct 2024)

This repository accompanies the master’s thesis:

> **"Occupation or Self-Defence? A Computational Analysis of NYT Framing, U.S. Foreign Policy, and Public Opinion"**  
> by **Kathia Reynoso**  
> MA in International Affairs and Diplomacy  
> UOC-UNITAR, 2025

This study analyzes how *The New York Times* framed the first year of the Israel-Hamas war and how its coverage aligned or diverged from U.S. government rhetoric and American public sentiment. The project combines Natural Language Processing (NLP) and qualitative content analysis to identify dominant frames, sentiment shifts, and correlations with foreign policy messaging.

---

## Setup

Clone the repository:

```bash
git clone https://github.com/kyreynoso/Is-it-Occupation-or-Self-defence-.git
```

### Requirements

Python 3.8+ with the following libraries:

* [spaCy](https://spacy.io/)
* [NLTK](https://www.nltk.org/)
* [gensim](https://radimrehurek.com/gensim/)
* [vaderSentiment](https://github.com/cjhutto/vaderSentiment)
* [scikit-learn](https://scikit-learn.org/stable/)
* [pandas](https://pandas.pydata.org/)
* [matplotlib](https://matplotlib.org/)
* [seaborn](https://seaborn.pydata.org/)

Install with:

```bash
pip install -r requirements.txt
```

## Methodology Overview

This project includes five key phases:

### 1. Data Collection

Web-scraped from [nytimes.com](https://www.nytimes.com/search/), [congress.gov](https://www.congress.gov/), and [presidency.ucsb.edu](https://www.presidency.ucsb.edu/)

Data includes 9,343 NYT articles, 229 White House statements, 124 Congressional Records

### 2. Sentiment Analysis

Using VADER to assess polarity over time by actor (Israel vs. Palestine)

### 3. Topic Modeling

Using LDA via `gensim` to extract dominant frames

### 4. Comparative Rhetoric Analysis

Alignment of NYT narratives vs. executive/congressional statements

### 6. Visualization

Time-series plots and actor-based framing shifts using `matplotlib` and `seaborn`



## Project Structure`
```bash
├── data/                    # Cleaned datasets (excluded in repo)
├── notebooks/               # Jupyter notebooks for analysis
├── scripts/                 
│   ├── preprocess_text.py
│   ├── sentiment_analysis.py
│   ├── topic_modeling.py
│   └── frame_alignment.py
├── visualizations/          # Graphs, charts, exportable visuals
├── requirements.txt
├── LICENSE
└── README.md
```


### Limitations
- Sentiment scoring tools may miss nuance (e.g., sarcasm or passive framing)

- Temporal correlations are observed, not causative

- Corpus is limited to English-language articles and U.S. government rhetoric

### Citation

If you use this repository, please cite:

Reynoso, Kathia. Is It Occupation or Self-Defence? A Computational Analysis of NYT Framing, U.S. Foreign Policy, and Public Opinion. MA Thesis, UOC-UNITAR, 2025. GitHub, https://github.com/kyreynoso/Is-it-Occupation-or-Self-defence-.

# Mapping Crypto Communities in r/CryptoMoonShots

This project analyzes discussions on **r/CryptoMoonShots** to uncover structure, relationships, and sentiment in the cryptocurrency ecosystem using **network science** and **NLP techniques**.

It builds a *co-mention network of cryptocurrencies* based on Reddit posts, detects communities, and analyzes them using TF–IDF and sentiment analysis.

---

## 📌 Project Overview

The pipeline performs the following steps:

1. **Data preprocessing**
   - Clean Reddit post titles and self-text
   - Remove URLs, emojis, punctuation, and noise
   - Tokenize and normalize text

2. **Ticker extraction**
   - Detect cryptocurrency tickers mentioned in posts
   - Normalize symbols and filter invalid tokens

3. **Network construction**
   - Build a *co-mention graph*:
     - Nodes → cryptocurrencies
     - Edges → coins mentioned together in the same post
   - Edge weight = number of co-occurrences

4. **Community detection**
   - Identify clusters of related cryptocurrencies
   - Reveal topical or hype-driven groupings

5. **Network analysis**
   - Centrality measures (degree, betweenness, etc.)
   - Structural properties of the graph
   - Identification of influential coins

6. **TF–IDF analysis**
   - Extract keywords representative of each community
   - Understand semantic focus of different clusters

7. **Sentiment analysis**
   - Compute sentiment scores for posts
   - Aggregate sentiment per coin and per community
   - Compare emotional tone across clusters

---

## 📂 Project Structure

```
.
├── notebook.ipynb        # Main analysis notebook
├── README.md             # Project documentation
└── data/                 # (Optional) Raw or processed Reddit data
```

---

## 🧠 Methods & Techniques

### NLP
- Text normalization & tokenization
- TF–IDF vectorization
- Sentiment analysis

### Network Science
- Graph construction from co-occurrences
- Community detection
- Centrality metrics
- Structural analysis

### Libraries Used
- Python
- pandas
- numpy
- networkx
- scikit-learn
- matplotlib / seaborn
- nltk / text processing tools

---

## 📊 Example Use Cases

- Discover emerging crypto narratives
- Identify tightly connected token ecosystems
- Detect hype-driven communities
- Combine sentiment + topology for market insight
- Research social dynamics in crypto forums

---

## 🚀 How to Run

1. Install dependencies:
```bash
pip install pandas numpy networkx scikit-learn matplotlib nltk
```

2. Open the notebook:
```bash
jupyter notebook notebook.ipynb
```

3. Run cells in order to reproduce the analysis.

---

## 📈 Possible Extensions

- Temporal network evolution
- Dynamic community tracking
- Integration with price data
- Reddit + Twitter fusion
- Graph embeddings (Node2Vec)
- Predictive models for trend detection

---

## 📜 License

This project is for research and educational purposes.

---

## ✨ Author

Guido Biosca  
Computer Engineering  
Focus on data science, networks, and applied machine learning

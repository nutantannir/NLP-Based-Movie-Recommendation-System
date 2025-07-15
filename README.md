### NLP-Based-Movie-Recommendation-System

🎬🎵 NLP-Based Cross-Domain Movie Recommendation System
This project is part of my MSc dissertation in Data Science at Middlesex University. It explores how advanced NLP techniques can bridge the gap between two distinct media domains—music and film—to recommend movies that are thematically and emotionally aligned with song lyrics.

📌 Project Overview
In a world flooded with content, this system aims to enhance discovery by linking songs and movies through shared sentiment, theme, and narrative depth.

💡 What It Does
Given a song title and artist, the system:

Analyzes the lyrics and computes semantic embeddings.

Matches it against a movie database using plot summaries, sentiment analysis, and keyword extraction.

Recommends the top 5 movies that are contextually and emotionally aligned with the song.

🧠 Technologies & Tools
NLP Models: Sentence-BERT (all-MPNet-base-v2)

Sentiment Analysis: TextBlob

Keyword Extraction: KeyBERT

Data Collection: Spotify API, Genius API, OMDB API

Similarity Metric: Cosine Similarity

Language: Python (Jupyter Notebooks)

📂 Dataset
Songs: ~1,495 curated tracks across 5 genres (Pop, Rock, Hip-Hop, R&B/Soul, Electronic)

Movies: ~1,501 films aligned with thematic elements in the songs

Includes custom features: sentiment polarity, keyword tokens, genre, and plot embeddings

🔍 Core Features
Feature	Description
Lyrics/Plot Embeddings	Uses Sentence-BERT to generate 768-dim embeddings
Sentiment Scores	Polarity score to capture emotional tone
Keyword Extraction	Extracts 5 most context-relevant terms per item
Weighted Similarity Matching	Combines semantic, emotional, and thematic features

🔬 Evaluation
Ablation Study to measure impact of each NLP feature

Baseline Comparison with TF-IDF-based system

Metrics: Diversity, Novelty, Cosine Similarity

User Survey: Gathered feedback on thematic accuracy and emotional coherence

📈 Results Summary
Outperformed TF-IDF baseline in thematic alignment and user satisfaction

Full system (BERT + Sentiment + Keywords) provided the most balanced, emotionally coherent, and novel recommendations

# 🔍 Author Profiling via Twitter Text Mining

> Análisis de datos y perfilado de autoría a través de tweets — UABC, 2022.

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-NLP-154F5B?style=flat)
![spaCy](https://img.shields.io/badge/spaCy-NLP-09A3D5?style=flat&logo=spacy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-data-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-visualization-11557C?style=flat)
![Status](https://img.shields.io/badge/status-academic%20project-blue?style=flat)
![Paper](https://img.shields.io/badge/paper-Overleaf%20LaTeX-47A141?style=flat&logo=overleaf&logoColor=white)

---

## 📌 Overview

Text mining project that extracts and analyzes Twitter data to build **behavioral and linguistic profiles** of public figures. Given a set of tweets from different authors, the system identifies writing patterns, vocabulary distribution, and stylistic features that allow distinguishing between authors — even when tweet content is unrelated.

**Authors analyzed:** Bill Gates · Elon Musk · Mayor Ed Lee  
**Total tweets processed:** ~7,173 across 3 authors (Aug 2012 – Nov 2017)

> 📄 Full methodology and results available in the **[academic paper (Spanish)](https://es.overleaf.com/read/brdkfyynbskh#707b21)** — written in IEEE format using LaTeX.

---

## 🎯 Problem Statement

Can we identify whether a Twitter account is authentic or impersonated by analyzing **writing patterns alone** — even from short texts like tweets?

This project explores that question by profiling 3 public figures across 75 months of activity, extracting stylometric features and visualizing behavioral differences between authors.

---

## 🔬 Methodology

```
Raw tweet data (Tweepy)
    └─► Data extraction & cleaning
            └─► Tokenization (NLTK / spaCy)
                    └─► Feature extraction
                            ├─► Word frequency per author
                            ├─► Unique vocabulary size
                            ├─► Tweets per month / day
                            ├─► Average tweet length
                            └─► Topic clustering
                                    └─► Author profiling & comparison
```

---

## 📊 Key Findings

| Author | Tweets/month | Words/month | Unique vocab |
|---|---|---|---|
| Bill Gates | 27.3 | 420 | 4,848 |
| Elon Musk | 46.98 | 589.63 | 6,628 |
| Mayor Ed Lee | 81.56 | 1,395.9 | 5,770 |

**Notable patterns identified:**
- **Elon Musk** — highest unique vocabulary; alternates between very short and long tweets; top words: Tesla, SpaceX, model, rocket
- **Bill Gates** — most balanced word distribution; humanitarian vocabulary despite tech background
- **Mayor Ed Lee** — highest activity during electoral campaigns; strongly location-anchored (SF, city, residents)

---

## ⚙️ Tech Stack

| Purpose | Technology |
|---|---|
| Data collection | Tweepy (Twitter API) |
| Data processing | Python, Pandas |
| NLP & tokenization | NLTK, spaCy |
| ML & analysis | scikit-learn, SciPy |
| Visualization | Matplotlib |
| Paper | LaTeX (Overleaf, IEEE format) |
| Notebook | Google Colab |

---

## 📁 Repository Structure

```
├── data_mining.ipynb         # Full analysis notebook (Google Colab)
└── data/                     # Not included due to Twitter API terms
    ├── elonmusk_tweets.txt
    ├── billgates_tweets.txt
    └── mayoredlee_tweets.txt
```

---

## 💡 Relevance & Applications

Author profiling via text mining has direct applications in:
- **Social listening & brand monitoring** — identifying authentic vs. inauthentic accounts
- **Disinformation detection** — flagging impersonation at scale
- **Audience segmentation** — understanding communication styles across demographics
- **Content intelligence** — extracting behavioral signals from unstructured text

---

## 📎 Academic Reference

- **Course:** Minería de Datos 2022-1 & 2022-2 — Facultad de Ciencias, UABC
- **Institution:** Universidad Autónoma de Baja California
- **Paper:** [Read on Overleaf](https://es.overleaf.com/read/brdkfyynbskh#707b21)
- **Notebook:** Available in this repository (`Mineria_de_Datos.ipynb`)

---

## 🔗 Related Projects

- [Edge-Telemetry-Pipeline](https://github.com/AlonsoDelRio/Edge-Telemetry-Pipeline) — Production IoT architecture with CI/CD
- [Bookmark Manager](https://github.com/AlonsoDelRio/bookmark-manager) — Full-stack app with FastAPI + React

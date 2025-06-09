# 📊 FinancialAnalysisProject

**Momentum Strategy and Portfolio Optimisation Report with Sentiment Analysis**

This repository contains a comprehensive dual-phase project focused on advanced financial analytics and natural language processing. It is divided into two main parts:

- **Part A**: Implementation and evaluation of sentiment analysis models to enhance recommendation systems.
- **Part B**: Development, backtesting, and optimisation of a momentum-based trading strategy on NASDAQ stocks (2014–2024), including portfolio construction.

---

## 📅 Table of Contents

- [📖 Introduction](#📖-introduction)  
- [📈 Part A: Sentiment Analysis](#📈-part-a-sentiment-analysis)  
  - [Objective](#objective)  
  - [Methodology](#methodology)  
  - [Models Evaluated](#models-evaluated)  
  - [Results](#results)  
  - [Proposed Enhancements](#proposed-enhancements)  
- [📁 Part B: Momentum Strategy](#📁-part-b-momentum-strategy)  
  - [Asset Overview](#asset-overview)  
  - [Momentum Strategy](#momentum-strategy)  
  - [Backtesting](#backtesting)  
  - [Strategy Optimisation](#strategy-optimisation)  
  - [COVID-19 Recovery Comparison](#covid-19-recovery-comparison)  
  - [Portfolio Optimisation](#portfolio-optimisation)  
- [📂 Files](#📂-files)    
- [📚 References](#📚-references)

---

## 📖 Introduction

This project explores two key areas in financial and data science:

- **Part A**: Investigates machine learning and deep learning models (SVM, Random Forest, CNN, LSTM) for sentiment classification. The goal is to improve content recommendation systems by integrating sentiment analysis based on user feedback.
- **Part B**: Applies quantitative techniques to implement and refine a momentum trading strategy. It also constructs an optimised investment portfolio using risk-return tradeoffs from 2014 to 2024.

---

## 📈 Part A: Sentiment Analysis

### Objective

To determine the most effective sentiment classification model and leverage sentiment data for personalised recommendation systems.

### Methodology

- **Preprocessing**: Text cleaning, tokenization, stopword removal, and TF-IDF vectorisation  
- **Training**: Evaluated both ML (SVM, Naive Bayes, Random Forest) and DL (CNN, LSTM) models  
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score

### Models Evaluated

| Model          | Highlights                                   |
|----------------|----------------------------------------------|
| SVM            | Strong with high-dimensional text data       |
| Naive Bayes    | Fast and scalable for large datasets         |
| Random Forest  | Good interpretability and generalisation     |
| CNN            | **Best accuracy** (73%)                      |
| LSTM           | Captures long-term dependencies moderately well |

### Results

- **CNN** achieved the highest and most balanced accuracy.
- **Random Forest** and **SVM** followed closely.
- **Naive Bayes** and **LSTM** underperformed on recall and F1-score.

### Proposed Enhancements

- Integrate user reviews and social media sentiment.
- Model temporal dynamics (e.g., seasonality, time-of-day).

---

## 📁 Part B: Momentum Strategy

### Asset Overview

Analysis covers 10 NASDAQ-listed stocks including: `EBAY`, `SBUX`, `NFLX`, `TSLA`, `MRNA`, and others using adjusted closing prices from **2014–2024**.

### Momentum Strategy

- **Strategy**: Simple Moving Average (SMA) Crossover  
- **Signal Logic**:  
  - **Buy**: Short-term SMA crosses above long-term SMA  
  - **Sell**: Reverse crossover  
- **Case Study**: Applied on `NFLX`

### Backtesting

- **Initial Capital**: $150,000  
- **Period**: 10 years  
- **Performance Metrics**:  
  - Sharpe Ratio  
  - Cumulative Returns  
  - Buy/Sell Signal Accuracy

### Strategy Optimisation

- **Optimised SMA Windows**: 30-day & 120-day  
- **Sharpe Ratio Improvement**: 0.2916 → **0.3548**

### COVID-19 Recovery Comparison

- **Fastest Recovery**: `MRNA`, `TSLA`  
- **Stable Recovery**: `GILD`, `COST`

### Portfolio Optimisation

- **Methodology**: Mean-Variance via `Riskfolio-Lib`  
- **Visualisations**:  
  - Efficient Frontier  
  - Asset Allocation Heatmaps  
- **Outcomes**:  
  - Sharpe-optimal portfolios  
  - CVaR-balanced allocations

---

## 📂 Files

- `Financial analysis.ipynb` – Complete notebook with code for Parts A and B  
- `Advanced_Analytics_Report.docx` – Detailed documentation and analysis  
- `README.md` – Project overview and guide (this file)

---

## 📚 References

- Liu (2012), Pang & Lee (2008), Breiman (2001), Kim (2014)  
- Hochreiter & Schmidhuber (1997), Jegadeesh & Titman (1993), Hyndman & Athanasopoulos (2018)  
- Medhat et al. (2014), McCallum & Nigam (1998), Zhou et al. (2019)

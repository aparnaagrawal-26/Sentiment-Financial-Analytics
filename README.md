📊 FinancialAnalysisProject

Momentum Strategy and Portfolio Optimisation Report with Sentiment Analysis

This repository contains a comprehensive project divided into two parts:

Part A: Implementation and evaluation of sentiment analysis models to enhance recommendation systems.

Part B: In-depth analysis of a momentum-based trading strategy, applied to select NASDAQ assets from 2014 to 2024. This part includes strategy backtesting, optimisation, and portfolio construction using modern financial techniques.

📅 Table of Contents

Introduction

Part A: Sentiment Analysis

Objective

Methodology

Models Evaluated

Results

Proposed Enhancements

Part B: Momentum Strategy

Asset Overview

Momentum Strategy

Backtesting

Strategy Optimisation

COVID-19 Recovery Comparison

Portfolio Optimisation

Files

How to Run

References

📖 Introduction

This dual-phase project focuses on two advanced analytics areas:

Part A investigates machine and deep learning models (SVM, Random Forest, CNN, LSTM) for sentiment classification, with a goal of enhancing content recommendation systems using user feedback.

Part B applies quantitative finance techniques to develop a robust momentum trading strategy and optimised investment portfolio from NASDAQ-listed stocks over a 10-year period.

📈 Part A: Sentiment Analysis

Objective

To identify the most effective sentiment analysis model and integrate user sentiment insights into recommendation systems for enhanced personalization.

Methodology

Preprocessing: Text cleaning, tokenization, stopword removal, TF-IDF vectorization

Training: ML (SVM, Naive Bayes, Random Forest) and DL (CNN, LSTM) models

Evaluation: Accuracy, precision, recall, F1-score

Models Evaluated

SVM: Effective in high-dimensional text data

Naive Bayes: Fast, suitable for large datasets

Random Forest: Good for interpretability and generalisation

CNN: Best overall accuracy (73%)

LSTM: Handles long-text dependencies moderately well

Results

CNN was the most accurate and balanced model. Random Forest and SVM followed closely. Naive Bayes and LSTM had lower recall and F1-scores.

Proposed Enhancements

Sentiment from User Reviews & Social Media

Incorporate Temporal Dynamics (e.g., seasonality, time-of-day activity)

📁 Part B: Momentum Strategy

Asset Overview

Analysis is conducted on 10 NASDAQ stocks (e.g., EBAY, SBUX, NFLX, TSLA, MRNA) using adjusted close prices from 2014 to 2024.

Momentum Strategy

Strategy: Simple Moving Average (SMA) Crossover

Signals: Buy when short-term SMA crosses above long-term; sell on the reverse

Case Study: NFLX

Backtesting

Initial capital: $150,000

10-year period

Metrics: Sharpe Ratio, Buy/Sell Signal Effectiveness, Cumulative Return

Strategy Optimisation

SMA windows tuned (e.g., 30-day & 120-day)

Sharpe Ratio improved from 0.2916 to 0.3548

COVID-19 Recovery Comparison

MRNA & TSLA rebounded fastest

GILD & COST showed steady but slower recoveries

Portfolio Optimisation

Method: Mean-Variance via Riskfolio-Lib

Visuals: Efficient Frontier, Asset Allocation Heatmaps

Result: Sharpe-optimal and CVaR-balanced portfolios

📂 Files

Financial analysis.ipynb: Notebook with full code for both parts

Advanced_Analytics_Report.docx: Detailed analysis and documentation

README.md: Project summary and guide (this file)

🚀 How to Run

Clone the repository:

git clone https://github.com/your-username/FinancialAnalysisProject.git
cd FinancialAnalysisProject

Install dependencies:

pip install -r requirements.txt

Launch Jupyter:

jupyter notebook

Run the cells in Financial analysis.ipynb

📚 References

Liu (2012), Pang & Lee (2008), Breiman (2001), Kim (2014)

Hochreiter & Schmidhuber (1997), Jegadeesh & Titman (1993), Hyndman & Athanasopoulos (2018)

Medhat et al. (2014), McCallum & Nigam (1998), Zhou et al. (2019)


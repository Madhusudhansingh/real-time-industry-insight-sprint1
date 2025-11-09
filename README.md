# Real-Time Industry Insight System — Sprint 1

This repository contains Sprint-1 of my Industry Insight project.  
The goal for this sprint was to build a small working slice of the system:
collect sample news data for three companies, run sentiment analysis, and generate basic outputs.

---

## ✅ Companies Covered in Sprint 1
- Infosys  
- Reliance Industries  
- TCS (Tata Consultancy Services)

Each company has 5 sample news headlines stored in the `data/` folder.

---

## ✅ Work Completed in Sprint-1

### 1) Data Preparation
- Created sample headline CSVs for all three companies:
  - `infosys_headlines.csv`
  - `reliance_headlines.csv`
  - `headlines_sample.csv` (TCS)
- All stored under the `data/` directory.

### 2) Sentiment Analysis
- Loaded all CSVs into a Google Colab notebook.
- Used a simple transformer sentiment model to analyze each headline.
- Extracted:
  - Sentiment label (positive / negative)
  - Confidence score
  - Signed score (positive = +score, negative = –score)

### 3) Final Combined Output
Saved a merged result file:
data/sentiment_results.csv

Columns in this file:
company, title, label, score, signed_score

---

## ✅ Output Charts (Saved in /outputs)

### **1. Sentiment Count by Company**
Shows how many positive/negative headlines each company has.  
File: `outputs/sentiment_counts_per_company_clean.png`

### **2. Average Sentiment Score**
Shows the average signed sentiment score for each company.  
File: `outputs/average_sentiment_score.png`

---

## ✅ Notebook Used
`sprint1_news_analysis.ipynb`  
This file contains the complete analysis:
- loading data  
- running sentiment model  
- merging results  
- generating charts  

You can open it in Google Colab and run everything end-to-end.

---

## ✅ How to Run (Quick Guide)

1. Open the notebook in Google Colab.  
2. Make sure CSV files inside `/data` are accessible (raw GitHub links or local).  
3. Run the notebook top-to-bottom.  
4. New outputs will be saved inside `/content/data` and `/content/outputs`.

---

## ✅ What’s Next (Sprint-2 Plan)
- Fetch real news from APIs  
- Automate repeated sentiment scoring  
- Set up notifications or alerts  
- Store results in a backend or Google Sheet  
- Improve charts and dashboard visuals  

---

## ✅ Repository Structure

real-time-industry-insight-sprint1/
│
├── data/
│   ├── infosys_headlines.csv
│   ├── reliance_headlines.csv
│   ├── headlines_sample.csv
│   └── sentiment_results.csv
│
├── outputs/
│   ├── sentiment_counts_per_company_clean.png
│   └── average_sentiment_score.png
│
├── sprint1_news_analysis.ipynb
└── README.md

# FinBERT Sentiment Analysis on E.ON Annual Reports

This repository contains the code and methodology for applying **FinBERT** (a financial BERT model) to analyze sentiment in E.ON's annual reports and sustainability disclosures from 2014 to 2025.

---

## Repository Structure

---

## Output Example

Each CSV file contains:

| Column | Description |
|--------|-------------|
| sentence | Original text from the PDF |
| sentiment | positive / negative / neutral |
| positive_score | Confidence score for positive |
| negative_score | Confidence score for negative |
| neutral_score | Confidence score for neutral |

---

## Methodology

1. Text Extraction using pypdf
2. Sentence Tokenization using NLTK punkt
3. FinBERT inference via Hugging Face
4. Export results to CSV

---

## Requirements
---

## How to Run

1. Place PDF files in the same folder as the notebook
2. Run finbert_analysis_EON.ipynb
3. Results saved in Output_Results/

---

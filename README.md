# FinBERT Sentiment Analysis on E.ON Annual Reports

This repository contains the code and methodology for applying **FinBERT** (a financial BERT model) to analyze sentiment in E.ON's annual reports and sustainability disclosures from 2014 to 2025.

---

## 📁 Repository Structure
MyAnalysis/
├── finbert_analysis_EON.ipynb # Main analysis notebook
└── Output_Results/ # Sentence-level sentiment CSV files

text

---

## 📊 Output Example

Each CSV file contains:

| Column | Description |
|--------|-------------|
| `sentence` | Original text from the PDF |
| `sentiment` | positive / negative / neutral |
| `positive_score` | Confidence score for positive |
| `negative_score` | Confidence score for negative |
| `neutral_score` | Confidence score for neutral |

---

## 🔧 Methodology

1. **Text Extraction**: Extract text from PDFs using `pypdf`
2. **Sentence Tokenization**: Split into sentences using NLTK's `punkt`
3. **Sentiment Analysis**: FinBERT inference via Hugging Face Transformers
4. **Export**: Save results to CSV with confidence scores

---

## 📦 Requirements

```bash
pip install pypdf transformers torch pandas numpy tqdm nltk

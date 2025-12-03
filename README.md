<div align="center">

# 🇸🇪 Swedish Language Datasets Collection

[![English](https://img.shields.io/badge/Lang-English-gray)](./README.md)
[![简体中文](https://img.shields.io/badge/Lang-简体中文-blue)](./README_zh.md)
[![Svenska](https://img.shields.io/badge/Lang-Svenska-blue)](./README_sv.md)

</div>

---

## 📖 Introduction
This repository contains a curated index of **60 publicly available Swedish language datasets**.
It details metadata such as source, applicable tasks, modality, and access links, designed to help NLP researchers and linguists quickly locate suitable Swedish corpora.

**Key Fields:**
- `Dataset Name`: Name of the dataset
- `Dataset Description`: Brief summary of contents
- `Tasks`: Applicable NLP tasks (e.g., Sentiment Analysis, POS tagging)
- `Modality`: Data type (Text, Speech, Image, etc.)
- `Citing/Cited Papers`: Related academic references

## 📊 Data Preview

> 💡 **Tip:** Click [swedish_dataset_list](./swedish_dataset_list) to view the full, searchable table.

Below is a preview of the first 5 entries:

| ID | Dataset Name | Modality | Tasks | Dataset Description |
| :--- | :--- | :--- | :--- | :--- |
| 9696 | ABSAbank-Imm | Text | language understanding | absabank-Imm is actually a sub-dataset included in the SuperLim-2 benchmark suite... |
| 9697 | ASU | Text | Natural Language Processing (NLP) | ASU is a Swedish written corpus built under the Språkbanken Text project... |
| 9698 | COCTAILL | Text | Natural Language Processing (NLP) | A textbook corpus for learners of Swedish as a second language (L2)... |
| 9699 | CoNLL17 corpus | Text | Part-of-speech tagging | CoNLL17 is a multilingual dependency parsing corpus covering 45 languages... |
| 9700 | Cross-linguistic Lexical Task (CLT) | Text, Speech, Image | Vocabulary comprehension assessment | A dataset of cross-linguistic vocabulary assessment tasks... |

*(Please download the CSV file to see all 60 datasets)*

## 🚀 Usage

### 1. Browse on GitHub
Simply click on the `swedish_dataset_list` file above to use GitHub's built-in table viewer with search and filter capabilities.

### 2. Load with Python
```python
import pandas as pd

# Load the dataset directly from GitHub
url = "[https://raw.githubusercontent.com/YOUR_USERNAME/REPO_NAME/main/swedish_dataset_list](https://raw.githubusercontent.com/YOUR_USERNAME/REPO_NAME/main/swedish_dataset_list)"
df = pd.read_csv(url)

# Example: Filter for 'Text' datasets
print(df[df['Modality'].str.contains('Text', na=False)].head())

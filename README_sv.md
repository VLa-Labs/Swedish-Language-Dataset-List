<div align="center">

# 🇸🇪 Samling av Svenska Datamängder

[![English](https://img.shields.io/badge/Lang-English-blue)](./README.md)
[![简体中文](https://img.shields.io/badge/Lang-简体中文-blue)](./README_zh.md)
[![Svenska](https://img.shields.io/badge/Lang-Svenska-gray)](./README_sv.md)

</div>

---

## 📖 Introduktion
Detta projekt innehåller metadata för **60** offentligt tillgängliga svenska datamängder.
Listan beskriver varje datamängds källa, tillämpbara uppgifter, modalitet och åtkomstlänkar, syftande till att hjälpa NLP-forskare att snabbt hitta lämpliga svenska korpusar.

**Huvudfält:**
- `Dataset Name`: Namn på datamängden
- `Dataset Description`: Kort beskrivning
- `Tasks`: Uppgifter (t.ex. NLP, POS-taggning)
- `Modality`: Datamodalitet (Text, Tal, Bild, etc.)
- `Citing/Cited Papers`: Akademiska referenser

## 📊 Förhandsgranskning (Data Preview)

> 💡 **Tips:** Klicka på [swedish_vocabulary.csv](./swedish_vocabulary.csv) för att se hela listan.

Nedan visas en förhandsgranskning av de första 5 raderna:

| ID | Dataset Name | Modality | Tasks | Dataset Description |
| :--- | :--- | :--- | :--- | :--- |
| 9696 | ABSAbank-Imm | Text | language understanding | absabank-Imm is actually a sub-dataset included in the SuperLim-2 benchmark suite... |
| 9697 | ASU | Text | Natural Language Processing (NLP) | ASU is a Swedish written corpus built under the Språkbanken Text project... |
| 9698 | COCTAILL | Text | Natural Language Processing (NLP) | A textbook corpus for learners of Swedish as a second language (L2)... |
| 9699 | CoNLL17 corpus | Text | Part-of-speech tagging | CoNLL17 is a multilingual dependency parsing corpus covering 45 languages... |
| 9700 | Cross-linguistic Lexical Task (CLT) | Text, Speech, Image | Vocabulary comprehension assessment | A dataset of cross-linguistic vocabulary assessment tasks... |

## 🚀 Användning

### Exempel med Python
```python
import pandas as pd

# Läs in datamängden
url = "[https://raw.githubusercontent.com/DITT_ANVÄNDARNAMN/REPO_NAMN/main/swedish_vocabulary.csv](https://raw.githubusercontent.com/DITT_ANVÄNDARNAMN/REPO_NAMN/main/swedish_vocabulary.csv)"
df = pd.read_csv(url)

# Exempel
print(df[['Dataset Name', 'Tasks']].head())

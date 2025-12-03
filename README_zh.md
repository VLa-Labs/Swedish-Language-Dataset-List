<div align="center">

# 🇸🇪 瑞典语数据集索引 (Swedish Datasets Collection)

[![English](https://img.shields.io/badge/Lang-English-blue)](./README.md)
[![简体中文](https://img.shields.io/badge/Lang-简体中文-gray)](./README_zh.md)
[![Svenska](https://img.shields.io/badge/Lang-Svenska-blue)](./README_sv.md)

</div>

---

## 📖 简介 (Introduction)
本项目整理了 **60 个** 与瑞典语（Swedish）相关的公开数据集元数据。
这份清单详细记录了每个数据集的来源、适用任务、模态（Modality）以及访问链接等信息，旨在帮助 NLP 研究者快速找到适合的瑞典语语料库。

**包含的主要字段：**
- `Dataset Name`: 数据集名称
- `Dataset Description`: 数据集简介
- `Tasks`: 适用任务 (如 NLP, Part-of-speech tagging 等)
- `Modality`: 数据模态 (Text, Speech, Image 等)
- `Citing/Cited Papers`: 相关学术引用

## 📊 数据预览 (Preview)

> 💡 **提示：** 点击 [swedish_dataset_list](./swedish_dataset_list) 可查看完整列表。

以下是精选的前 5 条数据预览：

| ID | Dataset Name | Modality | Tasks | Dataset Description |
| :--- | :--- | :--- | :--- | :--- |
| 9696 | ABSAbank-Imm | Text | language understanding | absabank-Imm is actually a sub-dataset included in the SuperLim-2 benchmark suite... |
| 9697 | ASU | Text | Natural Language Processing (NLP) | ASU is a Swedish written corpus built under the Språkbanken Text project... |
| 9698 | COCTAILL | Text | Natural Language Processing (NLP) | A textbook corpus for learners of Swedish as a second language (L2)... |
| 9699 | CoNLL17 corpus | Text | Part-of-speech tagging | CoNLL17 is a multilingual dependency parsing corpus covering 45 languages... |
| 9700 | Cross-linguistic Lexical Task (CLT) | Text, Speech, Image | Vocabulary comprehension assessment | A dataset of cross-linguistic vocabulary assessment tasks... |

*(更多数据请下载 CSV 文件查看)*

## 🚀 使用方法 (Usage)

### Python 读取示例
```python
import pandas as pd

# 读取数据集
url = "[https://raw.githubusercontent.com/您的用户名/仓库名/main/swedish_dataset_list](https://raw.githubusercontent.com/您的用户名/仓库名/main/swedish_dataset_list)"
df = pd.read_csv(url)

# 示例：筛选所有包含 "Text" 模态的数据集
print(df[['Dataset Name', 'Tasks']].head())

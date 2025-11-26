---
license: mit
task_categories:
- text-classification
- text-generation
- summarization
- text-retrieval
language:
- fa
tags:
- persian
- farsi
- nlp
- jumplander
- forum-data
- conversational
- community
- json
- ai-research
- iran-ai
- iran
- llm
- datasets
- data
- model
pretty_name: JumpLander Persian Forum Mini Dataset
size_categories:
- 1M<n<10M
---
# 📚 JumpLander Persian Forum Mini Dataset  
**High-Quality Persian (Farsi) Text for NLP and AI Research**

This dataset contains a **clean and structured subset of Persian community discussions** collected from JumpLander.org forums.  
It enables developers, researchers, and ML engineers to build and evaluate **Farsi NLP models** including:  
- Text classification  
- Topic modeling  
- Semantic search  
- NER / summarization  
- LLM and transformer fine-tuning

---

## 📊 Dataset Details

- **Language:** Persian (Farsi)  
- **Encoding:** UTF-8  
- **Source:** JumpLander Forum (https://jumplander.org)  
- **Format:** JSON (one file uploaded in this repository)  
- **Size:** Mini sample suitable for quick prototyping  
- **License:** Research / Non-Commercial (see License Notice below)

---

## 🧩 Data Schema

Every item contains:
```json
{
  "title": "عنوان نمونه",
  "slug": "sample-post",
  "content": "این یک متن نمونه برای آزمایش مدل‌های پردازش زبان است."
}
```

| Field | Type | Description |
|-------|------|-------------|
| `title` | `string` | Post title in Persian |
| `slug` | `string` | URL-friendly identifier (slug) |
| `content` | `string` | Clean body text extracted from forum posts (HTML removed) |

---

## 🚀 Quick Usage Example

### Load in Python (from the Hub)
```python
from datasets import load_dataset

ds = load_dataset("<username>/<dataset-name>")
print(ds['train'][0])
```

### Load local JSON file
```python
import json
with open("jumplander_mini.json", "r", encoding="utf-8") as f:
    data = json.load(f)
print(data[0])
```

### Convert to DataFrame
```python
import pandas as pd
df = pd.DataFrame(data)
print(df.head())
```

---

## 🔍 Applications

- AI Assistants: Persian chatbot training  
- Retrieval: Search/indexing engine fine-tuning  
- ML Experiments: Classification, topic clustering  
- LLM Evaluation: Benchmarks for Farsi text quality

This dataset represents **real conversational Persian** — informal, community-driven, modern writing.

---

## 🛡️ License Notice
This dataset is provided **for research and educational use only**.  
Please ensure compliance with the original website terms before any commercial use or republication. If in doubt, contact the dataset maintainer.

---

## 📚 Citation
If you use this dataset in your work, please cite it as:

**JumpLander Persian Forum Mini Dataset**. JumpLander.org. (Dataset).  

BibTeX:
```bibtex
@misc{jumplander2025,
  title = {JumpLander Persian Forum Mini Dataset},
  author = {{JumpLander Community / Dataset Curator}},
  year = {2025},
  howpublished = {\url{https://huggingface.co/<username>/<dataset-name>}}
}
```

---

## 🤝 Contribution & Support
Contributions, improvements, and issue reports are welcome.  
Maintainer: **<Your Name>**  
Contact: **<email or GitHub profile>**

---

## ✅ Notes for the Maintainer (replace placeholders)
- Replace `<username>/<dataset-name>` with your Hugging Face namespace and dataset name in examples.  
- Replace `jumplander_mini.json` with the actual file name you uploaded.  
- Update the License section if you have specific permissions or license details.

---
Thank you for preparing and sharing Persian language data — this dataset will help many researchers and developers working with Farsi NLP.

---


## 🔗 Stay Connected with JumpLander

Looking for more Persian NLP resources, community projects, or research collaborations?  
JumpLander is building the future of Farsi AI — together with developers like you.

👉 Visit us here: **[JumpLander.org](https://jumplander.org)**

Let’s push the boundaries of Persian language technology — one dataset at a time. 🚀✨

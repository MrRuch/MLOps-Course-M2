# MLOps – Course

This repository contains the slides, labs, and project scaffold for a  MLOps training:

## Structure
```
mlops_2day_course/
├── slides/
│   └── MLOps_SupdeVinci.pptx
├── labs/
│   ├── Lab1/
│   └── Lab2_SA_HuggingFace/
├── project/
│   └── ml_microservice/
├── docs/
│   └── syllabus.md

```

## Quickstart

This project aims to test some models provided by Hugging Face, starting with Sentiment Analysis.

👉 Trained model available here: [MrRichu/distilbert-imdb-sentiment-analysis](https://huggingface.co/MrRichu/distilbert-imdb-sentiment-analysis)

## Usage

```python
from transformers import pipeline

clf = pipeline("sentiment-analysis", model="MrRichu/distilbert-imdb-sentiment-analysis")
print(clf("I really enjoyed this movie!"))

# NLP News Classification in R: Topic & Credibility Classifier

[![Language: R](https://img.shields.io/badge/Language-R-276DC3?style=flat&logo=r&logoColor=white)]()
[![Method: Supervised NLP](https://img.shields.io/badge/Method-Supervised%20NLP-blueviolet?style=flat)]()
[![Framework: tidymodels](https://img.shields.io/badge/Framework-tidymodels-orange?style=flat)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview

This repository provides a **supervised NLP text classification pipeline in R** for classifying news articles by **topic** (e.g., health, politics, economy) and **credibility** (credible vs. misleading). It uses the `tidymodels` ecosystem with `textrecipes` for text feature engineering and supports multiple classification algorithms.

> **Related Projects:**
> - 🦠 [facebook-reactions-covid19-india](https://github.com/sawoodanwar/facebook-reactions-covid19-india) — PhD thesis
> - 🧠 [stm-social-media-r](https://github.com/sawoodanwar/stm-social-media-r) — Topic modeling
> - 🛨 [disinformation-detection-ml](https://github.com/sawoodanwar/disinformation-detection-ml) — ML disinformation classifier
> - 💬 [sentiment-lexicon-comparison](https://github.com/sawoodanwar/sentiment-lexicon-comparison) — Sentiment toolkit

---

## Research Objectives

- Classify news articles into predefined topic categories using supervised learning
- Build a credibility classifier distinguishing reliable from misleading news
- Apply TF-IDF and n-gram features with `textrecipes`
- Compare classifiers: Logistic Regression, Random Forest, SVM
- Evaluate with cross-validation: Accuracy, F1, AUC-ROC

---

## Classification Tasks

| Task | Labels | Method |
|---|---|---|
| **Topic classification** | Health, Politics, Economy, Science, Entertainment | Multi-class, LR / RF |
| **Credibility classification** | Credible / Misleading | Binary, LR / SVM |

---

## Repository Structure

```
nlp-news-classification-r/
├── scripts/
│   ├── 01_data_prep.R              # Load, clean, label encode
│   ├── 02_feature_engineering.R    # TF-IDF, n-grams via textrecipes
│   ├── 03_model_training.R         # tidymodels workflow: LR, RF, SVM
│   ├── 04_evaluation.R             # CV metrics, confusion matrix, ROC
│   └── 05_visualization.R          # Feature importance, ROC plots
├── data/
│   └── README.md
├── output/
│   ├── figures/
│   └── tables/
├── .gitignore
├── README.md
└── LICENSE
```

---

## Requirements

```r
install.packages(c(
  "tidymodels", "textrecipes", "tidytext",
  "ranger", "kernlab", "vip", "ggplot2", "yardstick"
))
```

---

## Author

**Sawood Anwar** — PhD in Humanities (Text and Communication Sciences), University of Urbino Carlo Bo
Defended: 22 September 2025 | Supervisor: Prof. Fabio Giglietto

- 🔗 [GitHub](https://github.com/sawoodanwar) | 💼 [LinkedIn](https://www.linkedin.com/in/sawood-anwar/) | 🎓 [Google Scholar](https://scholar.google.com/citations?hl=en&user=GgsMu3sAAAAJ)

---

## License
MIT License. See [LICENSE](LICENSE).

*Keywords: Text Classification, NLP, tidymodels, textrecipes, News Credibility, Topic Classification, R, Supervised Learning, Computational Communication*

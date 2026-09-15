# phishing-detection-paper
Detecting Phishing URLS using URL-based and Webpage-based  Features

# Detecting Phishing URLs Using Machine Learning

[![Paper PDF](https://img.shields.io/badge/Paper-Download_PDF-blue.svg)](https://github.com/PizzaPower55/phishing-detection-paper/blob/main/Detecting%20Phishing%20URLS.pdf)
[![Open In Colab](https://img.shields.io/badge/Open_In-Colab-orange.svg?logo=googlecolab)](https://colab.research.google.com/drive/1Tv1kWjYUqDtIhV3rHifbNSgaN4LxPkmg)

A comparative study evaluating machine learning models (Random Forest, Decision Tree, KNN, Logistic Regression, MLP) on URL-based and webpage-based features for real-time phishing detection using the PhiUSIIL dataset.

---

## Key Findings

* **URL-Only High Performance:** Using only lexical and structural URL features, **Random Forest achieved 99.922% accuracy and 100% recall** (0 false negatives).
* **Proactive Security:** Detecting threats purely from URL structure enables preemptive blocking **before** a user lands on or loads a malicious webpage.
* **Webpage Feature Evaluation:** Webpage-level HTML features (e.g., metadata, external refs, forms) yielded up to **99.336% accuracy**, serving as a reliable secondary signal.

---

## Dataset & Model Performance

Evaluated on the **PhiUSIIL Phishing URL Dataset** (235,795 labeled samples).

### URL-Based Features Performance
| Model | Accuracy | Precision | Recall | F1 Score |
| :--- | :---: | :---: | :---: | :---: |
| **Random Forest** | **99.922%** | **99.863%** | **100.0%** | **99.932%** |
| K-Nearest Neighbors ($k=10$) | 99.892% | 99.812% | 100.0% | 99.906% |
| MLP Classifier (10, 5) | 99.809% | 99.668% | 100.0% | 99.834% |
| Decision Tree (max depth 6) | 99.729% | 99.529% | 100.0% | 99.764% |
| Logistic Regression | 99.599% | 99.313% | 99.993% | 99.652% |

---

## Requirements & Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/PizzaPower55/phishing-detection-paper.git
   cd phishing-detection-paper

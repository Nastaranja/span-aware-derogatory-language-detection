# Detecting Derogatory Language Usage with a Span-Aware Transformer

A Natural Language Processing (NLP) project exploring derogatory language detection through traditional machine learning, transformer-based classification, and unsupervised text clustering.

## Project Overview

This project investigates the detection of derogatory (DEG) language in online discussions using the Slur Corpus (Kurrek, Saleem & Ruths, 2020), containing 40,003 annotated Reddit comments.

The study compares traditional machine learning approaches with contextualized transformer models, including a CLS-only XLM-R baseline and a span-aware RAPT architecture.

Additionally, K-Means clustering is applied to learned text embeddings to explore whether semantic representations capture patterns associated with the target labels.

## Dataset

**Slur Corpus (Kurrek, Saleem & Ruths, 2020)**

- Total comments: 40,003
- Source: Reddit
- Task: Binary text classification
- Target classes:
  - DEG (Derogatory)
  - Non-DEG (Non-Derogatory)

## Methodology

### 1. Text Classification

We compare traditional machine learning methods against transformer-based approaches.

**Traditional Machine Learning**
- TF-IDF + Logistic Regression
- TF-IDF + Linear Support Vector Machine (SVM)

**Transformer-Based Models**
- XLM-R CLS-only baseline
- Span-aware RAPT architecture

### 2. Text Clustering

K-Means clustering is performed on learned embeddings to investigate the semantic structure of the comments.

The resulting clusters are evaluated against the ground-truth DEG and Non-DEG labels.

## Models and Techniques

| Component | Methods |
|---|---|
| Text Representation | TF-IDF |
| Classification | Logistic Regression |
| Classification | Linear SVM |
| Transformer | XLM-R |
| Architecture | Span-aware RAPT |
| Clustering | K-Means |

## Repository Structure

```text
span-aware-derogatory-language-detection/
│
├── README.md
├── text_mining_raptnew.ipynb
├── TMS_Project_Report.pdf
└── TMS_Presentation.pptx
```

## Project Files

- **Jupyter Notebook:** Source code and experimental implementation.
- **Project Report:** Detailed methodology, results, evaluation, and discussion.
- **Presentation:** Summary of the research project and its findings.

## Technologies

- Python
- Jupyter Notebook
- Natural Language Processing (NLP)
- Scikit-learn
- TF-IDF
- Transformer Models
- XLM-R
- Logistic Regression
- Support Vector Machines
- K-Means Clustering

## Research Objectives

1. Compare traditional machine learning and transformer-based classification approaches.
2. Investigate span-aware representations for derogatory language detection.
3. Evaluate contextualized text representations.
4. Explore semantic patterns through unsupervised clustering.

## Results and Evaluation

The experimental results, model comparisons, evaluation metrics, and detailed discussion are documented in the full project report.

## Ethical Considerations

This project addresses potentially harmful and offensive language in online communities.

The dataset and model outputs should be handled responsibly. The project is intended for research and analysis, not for generating or promoting harmful content.

Please refer to the original dataset documentation and licensing conditions before redistributing the data.

## References

Kurrek, J., Saleem, H. M., & Ruths, D. (2020). *Slur Corpus*.

---

**Project Repository:** [GitHub](https://github.com/Nastaranaja/span-aware-derogatory-language-detection)

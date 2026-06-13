# NOVA Food Classification Using Machine Learning and Transformer-Based NLP Techniques

An end-to-end Machine Learning and Natural Language Processing (NLP) framework for automated NOVA food classification using nutritional attributes, ingredient information, and food descriptions from the **USDA Food and Nutrient Database for Dietary Studies (FNDDS)**.

## Project Background

This project was developed under the guidance of **Prof. Ganesh Bagler (IIIT-Delhi)** and extends previously published research on automated NOVA food classification. Building upon the original framework, we explored additional feature engineering techniques, transformer-based language representations, class imbalance handling strategies, and robust validation methodologies.

The project investigates how structured nutritional information and unstructured textual data can be leveraged to improve automated classification of food products into NOVA processing categories.

## Related Publication:
https://scholar.google.com/citations?view_op=view_citation&hl=en&user=qyth_0QAAAAJ&citation_for_view=qyth_0QAAAAJ:w2UhwfzvF0QC

## Key Contributions

* Advanced feature engineering using nutritional and textual food attributes
* Correlation-based feature analysis and feature reduction
* Class imbalance handling using SMOTE
* Stratified K-Fold Cross-Validation for robust model assessment
* Evaluation of multiple Machine Learning models using engineered nutritional features
* Investigation of transformer-based NLP representations for food descriptions and ingredient information
* Performance assessment using Accuracy, Precision, Recall, F1 Score, and Matthews Correlation Coefficient (MCC)

---

## Dataset

**Source:** USDA Food and Nutrient Database for Dietary Studies (FNDDS)

The dataset contains comprehensive information about food products, including:

* Nutritional composition
* Food descriptions
* Ingredient-related information
* Dietary attributes

These structured and unstructured features were utilized to develop machine learning and NLP-based models for automated NOVA classification.

---

## Machine Learning Models Evaluated

* Logistic Regression
* Naive Bayes
* K-Nearest Neighbors (KNN)
* Decision Tree
* Random Forest
* Extra Trees Classifier
* AdaBoost
* Gradient Boosting
* XGBoost
* Support Vector Machine (SVM)
* Multi-Layer Perceptron (MLP)

---

## NLP Models and Embeddings

To capture semantic information from food descriptions and ingredient lists, transformer-based language models were employed:

* DistilBERT
* RoBERTa
* GPT-2

The generated embeddings were used to investigate the effectiveness of contextual language representations for automated NOVA classification.

---

## Evaluation Metrics

Model performance was evaluated using:

* Accuracy
* Precision
* Recall
* Weighted F1 Score
* Macro F1 Score
* Matthews Correlation Coefficient (MCC)
* Confusion Matrix Analysis

---

## Methodology

Dataset Collection

↓

Data Cleaning & Preprocessing

↓

Feature Engineering

↓

Train-Test Split

↓

Stratified K-Fold Cross Validation

↓

SMOTE (Applied to Training Folds Only)

↓

Model Training

↓

Performance Evaluation

↓

Results Analysis

---

## Results

The project evaluates multiple machine learning and transformer-based NLP approaches for NOVA food classification. Experimental findings demonstrate the impact of feature engineering, class balancing, and contextual language representations on classification performance.

Detailed performance metrics, confusion matrices, and model outputs are available in the accompanying notebooks and results directory.

---

## Repository Structure

```text
.
data/
├── numerical/
└── textual/
notebooks/
├── ML_Pipeline/
│   ├── 01_EDA.ipynb
│   ├── 02_Feature_Selection_and_Training.ipynb
│   └── 03_Stratified_KFold_Validation.ipynb
│
└── NLP_Pipeline/
    ├── 04_RoBERTa_Embeddings.ipynb
    ├── 05_DistilBERT_Embeddings.ipynb
    └── 06_GPT2_Embeddings.ipynb

├── README.md
└── requirements.txt
```

---

## Future Work

* Ensemble learning combining nutritional and transformer-based features
* Explainable AI techniques (SHAP, LIME)
* Domain-specific food language models
* Multimodal deep learning architectures
* Large Language Model (LLM)-based nutrition intelligence systems

---

## Acknowledgements

I would like to express my sincere gratitude to **Prof. Ganesh Bagler** for his guidance and mentorship throughout this project. This work extends previously published research from the lab and incorporates additional experimentation in feature engineering, validation methodologies, and transformer-based NLP approaches for automated NOVA food classification.

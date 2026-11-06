# Week 6: Model Evaluation and Business Insights

## Project Overview
This week focuses on evaluating machine learning models developed for sentiment classification of Amazon Beauty product reviews. The objective is to compare different models, identify the best-performing model, and derive meaningful business insights from customer feedback.

## Dataset
- **Dataset:** Amazon Beauty Reviews
- **Total Cleaned Reviews:** 10,192
- **Features:** Review text, ratings, product information, and engineered features.
- **Sentiment Labels:**
  - Negative: Ratings 1–2
  - Neutral: Rating 3
  - Positive: Ratings 4–5

## Models Evaluated
The following four models were evaluated:

1. Logistic Regression
2. Multinomial Naive Bayes
3. Decision Tree
4. Balanced Naive Bayes

TF-IDF was used for text feature extraction with a maximum of 5,000 features. The dataset was divided into training and testing sets using an 80:20 stratified split.

## Model Evaluation Metrics
Models were compared using:
- Accuracy
- Precision
- Recall
- Weighted F1-Score
- Macro F1-Score
- Macro ROC-AUC

Confusion matrices and performance comparison graphs were also generated to understand model performance across sentiment classes.

## Key Results

| Model | Accuracy | Weighted F1 | Macro F1 | Macro ROC-AUC |
|---|---:|---:|---:|---:|
| Logistic Regression | 77.49% | 79.66% | 57.31% | 0.8540 |
| Multinomial Naive Bayes | 73.17% | 76.91% | 56.24% | 0.8476 |
| Decision Tree | 70.03% | 72.68% | 45.11% | 0.6447 |
| Balanced Naive Bayes | 73.17% | 76.91% | 56.24% | 0.8476 |

## Best Performing Model
Logistic Regression achieved the best overall performance among the evaluated models, with:
- Accuracy: 77.49%
- Weighted F1-Score: 79.66%
- Macro F1-Score: 57.31%
- Macro ROC-AUC: 0.8540

However, performance on minority sentiment classes (Negative and Neutral) remains a challenge due to class imbalance.

## Business Insights
- Negative reviews can help identify customer complaints and product improvement areas.
- Positive reviews can reveal product strengths and customer satisfaction drivers.
- Neutral reviews can highlight areas where customer expectations are not fully met.
- Businesses can use sentiment trends to monitor customer feedback and support decision-making.
- Automated predictions should be reviewed by humans before important business decisions.

## Project Deliverables
This folder contains:
- Detailed model evaluation report (DOCX)
- Jupyter Notebook containing model evaluation
- Model evaluation results (CSV)
- ROC-AUC results (CSV)
- Graphs and visualizations
- Confusion matrices for all four models

## Limitations
- The dataset contains an imbalance between positive, neutral, and negative reviews.
- Rating-based sentiment labels may not always represent the actual meaning of review text.
- Sarcasm and contextual meaning may be difficult to identify.
- Model performance may vary on different datasets.
- Sentiment classification does not determine product safety or effectiveness.

## Conclusion
Week 6 successfully compared four machine learning models for sentiment classification. Logistic Regression demonstrated the strongest overall performance. The evaluation highlights the importance of considering multiple metrics, especially when dealing with imbalanced datasets. The resulting insights can help beauty and wellness businesses better understand customer feedback and identify opportunities for improvement.

---
**Internship:** Yuva Data Science Internship  
**Domain:** Beauty & Wellness  
**Week:** 06 – Model Evaluation and Business Insights

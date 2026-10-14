# Week 2: Data Identification, Sourcing Strategy & Initial Analysis Planning

## 1. Project Overview

**Project Title:** Customer Sentiment Analysis of Beauty Product Reviews

The objective of this project is to analyze customer reviews of beauty products to understand opinions, satisfaction levels, and common complaints. Data science techniques will be used to identify sentiment patterns and generate useful insights for the beauty and wellness industry.

## 2. Data Requirements

The project requires customer review data containing review text and product ratings. Additional fields such as product name, product category, review date, and verified-purchase status may be useful if available.

## 3. Potential Data Sources

### Source 1: Amazon Beauty Reviews
- Platform: Hugging Face
- Link: https://huggingface.co/datasets/jhan21/amazon-beauty-reviews-dataset
- Expected data: Customer reviews, ratings, product identifiers, and related review information.
- Advantage: Potentially provides a large collection of beauty-product feedback.
- Limitation: Large files may require sampling, and the actual schema and license must be verified.

### Source 2: Sephora Products and Skincare Reviews
- Platform: Kaggle
- Link: https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews
- Expected data: Beauty-product details, customer reviews, and ratings.
- Advantage: Focuses on beauty and skincare products.
- Limitation: Access may require a Kaggle account, and data usage terms must be checked.

### Source 3: Sephora Skincare Reviews and Sentiment
- Platform: Hugging Face
- Link: https://huggingface.co/datasets/haoxianc/natashamessier_sephora-skincare-reviews-and-sentiment
- Expected data: Skincare reviews and sentiment-related information.
- Advantage: A focused dataset that may be suitable for an initial analysis.
- Limitation: Coverage is limited to skincare, and existing sentiment labels require validation.

## 4. Dataset Selection Criteria

The datasets will be evaluated using the following criteria:

- **Relevance:** The data must relate to beauty and wellness products.
- **Accessibility:** The dataset should be publicly accessible.
- **Completeness:** Review text and ratings should have minimal missing values.
- **Quality:** Duplicate, irrelevant, and inconsistent records should be identified.
- **Format:** The data should be available in a format that Python tools can process.
- **License:** Usage restrictions must be reviewed before using the dataset.

## 5. Preliminary Data Source Selection

Amazon Beauty Reviews is the preferred candidate because of its potential coverage of a wide range of beauty products and customer opinions. However, the final dataset will be selected only after verifying the available files, column names, data quality, accessibility, and license.

## 6. Initial Analysis Plan

The planned analysis includes examining the number of reviews, rating distributions, missing values, duplicate records, and the frequency of positive and negative opinions. Text preprocessing and visualizations will help identify common words, customer concerns, and sentiment patterns.

Python libraries such as Pandas, NumPy, Matplotlib, Seaborn, and suitable natural language processing tools may be used.

## 7. Responsible Data Use

Only data that can be used under the applicable dataset license and terms will be selected. Unnecessary personal information will not be collected or analyzed. Dataset limitations and potential biases will be documented.

## 8. Expected Outcome

This document establishes a preliminary strategy for identifying and selecting a suitable dataset. It provides a foundation for data acquisition, quality assessment, exploratory data analysis, and future sentiment analysis.

The next stage will involve inspecting the selected dataset and confirming whether it meets the project's requirements.

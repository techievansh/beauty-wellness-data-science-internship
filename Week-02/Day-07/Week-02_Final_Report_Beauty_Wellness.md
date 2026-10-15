# Week 2 Final Report
## Data Identification, Sourcing Strategy and Initial Analysis Planning

**Project Title:** Customer Sentiment Analysis of Beauty Product Reviews  
**Industry:** Beauty and Wellness  
**Week:** 2

## 1. Introduction

The beauty and wellness industry includes skincare, haircare, cosmetics, and personal care products. Customers share their experiences through online reviews and ratings. Analysing these reviews can help businesses understand customer satisfaction, identify common complaints, and recognise areas for improvement.

This report presents the data identification, sourcing strategy, dataset evaluation, data quality assessment, and initial exploratory analysis plan for the project.

## 2. Problem Statement

Beauty product businesses receive large volumes of online customer reviews. Manually analysing these reviews can be time-consuming and make it difficult to identify common customer opinions.

This project aims to explore customer sentiment using written reviews and star ratings. The initial focus is to understand rating patterns, identify positive and negative feedback, and assess whether the available data is suitable for further sentiment analysis.

## 3. Project Objectives

- Identify publicly available beauty product review datasets.
- Compare potential data sources and their suitability.
- Establish a structured data collection strategy.
- Assess dataset relevance, accessibility, and potential quality issues.
- Identify important variables for analysis.
- Plan descriptive statistics, visualisations, and preprocessing.
- Establish how the data may help evaluate the project's hypotheses.

## 4. Potential Data Sources

### 4.1 Amazon Beauty Reviews Dataset

**Link:** https://huggingface.co/datasets/jhan21/amazon-beauty-reviews-dataset

The inspected preview contains customer ratings, review titles, review text, image metadata, product identifiers, timestamps, helpful votes, and verified purchase indicators.

**Advantages:**
- Includes written customer feedback and ratings.
- Contains several fields relevant to exploratory analysis.
- Can support investigation of rating patterns and review language.

**Limitations:**
- Missing values, duplicates, and overall data quality require quantitative checks.
- Licensing and permitted usage must be verified.
- The preview alone does not establish the quality of the complete dataset.

### 4.2 Sephora Products and Skincare Reviews

**Link:** https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews

This is a potential alternative for beauty product and skincare review analysis.

**Advantages:**
- Relevant to skincare and beauty products.
- May include product attributes alongside customer reviews.

**Limitations:**
- Account access may be required.
- The available columns, completeness, and licensing require verification.

### 4.3 Sephora Skincare Reviews and Sentiment

**Link:** https://huggingface.co/datasets/haoxianc/natashamessier_sephora-skincare-reviews-and-sentiment

This is another candidate for investigating skincare reviews and sentiment-related information.

**Advantages:**
- Relevant to customer sentiment analysis.
- May provide sentiment labels for comparison.

**Limitations:**
- The structure and method used to generate labels must be checked.
- Label quality, coverage, and licensing require verification.

### 4.4 Other Potential Sources

Official APIs, government open-data portals, and public social media data may provide additional information about consumer behaviour and beauty industry trends. Their usefulness depends on data availability, access permissions, coverage, and relevance to individual customer reviews.

## 5. Comparative Dataset Evaluation

The datasets were considered against relevance, accessibility, availability of review text, potential data quality, and usage permissions.

| Criterion | Amazon Beauty Reviews | Sephora Kaggle | Sephora Sentiment |
|---|---|---|---|
| Beauty industry relevance | High | High | High |
| Review text | Observed in preview | Verify | Verify |
| Ratings | Observed in preview | Verify | Verify |
| Accessibility | Public hosting page | Account may be required | Public hosting page |
| Data quality | Requires measurement | Requires inspection | Requires inspection |
| Licensing | Verify | Verify | Verify |

This is a preliminary comparison rather than a completed quantitative audit.

## 6. Selected Dataset and Sourcing Strategy

The Amazon Beauty Reviews dataset is the preliminary choice because the inspected sample contains review text, ratings, and supporting fields relevant to the project.

The proposed collection process is:

1. Review the dataset description, files, and available columns.
2. Verify the licence and usage conditions.
3. Load a manageable sample for initial inspection.
4. Check whether the required variables are present.
5. Measure missing values, duplicates, and invalid records.
6. Record the data access method and known limitations.
7. Retain a backup dataset if the primary source is unsuitable.

Only data needed for the project should be collected. Platform restrictions and applicable privacy requirements must be respected.

## 7. Key Variables

- **Rating:** Numerical customer rating.
- **Review Text:** Written feedback for text analysis.
- **Review Title:** Additional review context.
- **Timestamp:** Review date for potential temporal analysis.
- **Helpful Votes:** A measure of review engagement.
- **Verified Purchase:** Purchase verification indicator.
- **Product Identifier:** Enables grouping reviews by product.

The availability and completeness of these variables will be checked before analysis.

## 8. Data Quality Assessment and Preprocessing

The following checks are planned:

- Identify missing or empty review text.
- Detect duplicate records and repeated reviews.
- Validate ratings against the dataset's documented scale.
- Check missing product identifiers and review titles.
- Parse timestamps and examine date consistency.
- Inspect unusually short, irrelevant, or low-information reviews.
- Examine helpful-vote distributions and potential outliers.
- Standardise whitespace and handle encoding issues.
- Tokenise review text where required for text analysis.

Preprocessing decisions will be documented, and meaningful text such as negation words should be preserved when relevant to sentiment.

No dataset-wide missing-value percentages or duplicate counts are claimed at this planning stage.

## 9. Initial Exploratory Data Analysis Plan

### Descriptive Statistics

The analysis will examine:
- Total number of records.
- Rating frequencies and percentages.
- Mean, median, minimum, and maximum ratings.
- Missing-value counts and percentages.
- Review-length distribution.
- Helpful-vote distribution.
- Verified purchase proportions.
- Review counts over time, if timestamps are suitable.

### Planned Visualisations

- Bar chart of rating distribution.
- Histogram of review lengths.
- Box plot of review length by rating group.
- Histogram or box plot of helpful votes.
- Grouped bar chart comparing verified and unverified purchases.
- Line chart of review volume over time, if appropriate.
- Bar chart of frequent review terms.

### Statistical Methods

Frequency tables, percentages, descriptive statistics, quartiles, and suitable correlation or group-comparison methods will be considered. Statistical tests will be selected only after the data and relevant assumptions have been examined.

## 10. Hypotheses and Their Evaluation

**H1:** Higher-rated reviews are expected to contain more positive language.  
*Evaluation:* Compare review language across rating groups.

**H2:** Lower-rated reviews are expected to contain more complaints.  
*Evaluation:* Examine common terms and themes in lower-rated reviews.

**H3:** Review length may differ across rating groups.  
*Evaluation:* Compare review-length distributions.

**H4:** Helpful votes may vary with rating and review length.  
*Evaluation:* Explore relationships between helpful votes and selected variables.

These hypotheses remain untested until the planned analysis is performed. Star ratings are only an approximate indicator of sentiment and may not always match the written review.

## 11. Tools and Technologies

- Python
- Google Colab
- Pandas
- Matplotlib
- Seaborn
- Suitable natural language processing libraries

These tools can support data inspection, cleaning, descriptive analysis, visualisation, and later sentiment exploration.

## 12. Risks and Limitations

Potential limitations include biased customer participation, missing or duplicated records, incomplete product coverage, noisy review text, and disagreement between written sentiment and numerical ratings.

Public availability does not automatically grant unrestricted usage. Dataset licences, attribution requirements, and platform restrictions must be checked before collection or redistribution.

## 13. Conclusion

This report establishes a structured approach for identifying, evaluating, and sourcing data for customer sentiment analysis in the beauty and wellness industry. The Amazon Beauty Reviews dataset is the preliminary selection because its inspected preview contains relevant review and rating fields.

Further quantitative data quality checks are necessary before finalising the dataset for analysis. The proposed EDA and preprocessing plan will guide subsequent work and help evaluate the project's hypotheses.

## 14. References

1. Amazon Beauty Reviews Dataset — https://huggingface.co/datasets/jhan21/amazon-beauty-reviews-dataset
2. Sephora Products and Skincare Reviews — https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews
3. Sephora Skincare Reviews and Sentiment — https://huggingface.co/datasets/haoxianc/natashamessier_sephora-skincare-reviews-and-sentiment

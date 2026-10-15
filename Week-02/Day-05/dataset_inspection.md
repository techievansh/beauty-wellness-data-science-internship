# Dataset Inspection and Data Quality Report

## 1. Project Title
Customer Sentiment Analysis of Beauty Product Reviews

## 2. Objective
The objective is to inspect the selected dataset's structure, understand its important variables, and identify data quality checks required before exploratory data analysis.

## 3. Dataset Information

**Dataset:** Amazon Beauty Reviews Dataset

**Platform:** Hugging Face

**Link:** https://huggingface.co/datasets/jhan21/amazon-beauty-reviews-dataset

The dataset preview was inspected to understand its available columns and sample records. The observations below are based on the displayed preview and do not represent a complete audit of the entire dataset.

## 4. Observed Columns

| Column | Description | Potential Use |
|---|---|---|
| rating | Numerical customer rating | Rating distribution and preliminary sentiment grouping |
| title | Review headline | Additional review context |
| text | Written review | Text analysis and sentiment exploration |
| images | Associated image information | Optional review metadata |
| asin | Product identifier | Product-level grouping |
| parent_asin | Parent product identifier | Grouping related product variations |
| user_id | Reviewer identifier | Potential reviewer-level analysis, subject to privacy considerations |
| timestamp | Review date and time | Temporal analysis |
| helpful_vote | Number of helpful votes | Review engagement analysis |
| verified_purchase | Purchase verification indicator | Comparing verified and unverified reviews |

## 5. Initial Observations

The displayed sample contained ratings ranging from 1 to 5. Review text varied in length and included both positive experiences and complaints about product characteristics such as smell, quality, or usability.

The preview also showed Boolean values for `verified_purchase`, numerical values for `helpful_vote`, and image information that could be empty for some records.

These observations indicate that the dataset contains fields relevant to the project's initial analysis.

## 6. Planned Data Quality Checks

### Missing Values
- Count missing review titles and review text.
- Identify empty or whitespace-only reviews.
- Check missing ratings and product identifiers.

### Duplicate Records
- Check for exact duplicate records.
- Check for repeated review text and identifiers where appropriate.
- Avoid removing legitimate repeated opinions without further investigation.

### Rating Validation
- Confirm that ratings follow the dataset's documented rating scale.
- Investigate invalid or unexpected rating values.

### Text Quality
- Identify extremely short or irrelevant reviews.
- Check unusual characters, excessive whitespace, and encoding issues.
- Plan text normalisation if required for later analysis.

### Timestamp Validation
- Check whether timestamps can be parsed correctly.
- Identify missing or invalid dates.
- Examine the date range before performing temporal analysis.

### Other Checks
- Review the distribution of verified purchases.
- Examine helpful-vote values and potential outliers.
- Assess whether image metadata is necessary for the project.

## 7. Preliminary Sentiment Labelling

Customer ratings may provide an approximate reference for sentiment exploration. For example, high ratings may be treated as a preliminary indicator of positive sentiment and low ratings as a preliminary indicator of negative sentiment.

However, rating thresholds must be defined before analysis. Middle ratings may represent mixed or neutral opinions, and the written review should be considered when interpreting sentiment.

## 8. Privacy and Data Limitations

Reviewer identifiers should not be used to identify individuals. Only fields necessary for the analysis should be retained. Data access and processing must comply with the dataset's licence and applicable requirements.

The sample preview alone cannot establish overall missing-value percentages, duplicate counts, or the full dataset's representativeness. These must be measured during actual analysis.

## 9. Conclusion
The dataset preview contains useful variables for beauty product sentiment analysis. Before proceeding, quantitative quality checks should be performed to establish data completeness, consistency, and suitability for exploratory analysis.

# Variables and Data Requirements

## 1. Introduction

The selected business problem is Customer Sentiment Analysis of Beauty Product Reviews. To analyze customer feedback, we need to identify the important variables, understand their purpose, and define the data required for the analysis.

## 2. Required Data

The project will use publicly accessible beauty product review data. The preferred dataset should contain review text, customer ratings, and product information. Additional fields will be used where available.

## 3. Key Variables

| Variable | Description | Type | Purpose |
|---|---|---|---|
| Product ID | Unique identifier for a product | Categorical/Identifier | Group reviews by product |
| Product Name | Name of the beauty product | Text/Categorical | Identify products |
| Product Category | Type of product, such as skincare or makeup | Categorical | Compare categories |
| Rating | Customer's numerical product rating | Numerical/Ordinal | Analyze satisfaction |
| Review Title | Short heading of the review | Text | Identify key opinions |
| Review Text | Full written customer feedback | Text | Perform sentiment and theme analysis |
| Review Date | Date the review was submitted | Date/Time | Analyze changes over time |
| Reviewer ID | Available reviewer identifier, preferably anonymized | Identifier | Assess repeat reviews where appropriate |
| Sentiment | Positive, negative, or neutral label | Categorical | Analyze customer opinion |
| Review Length | Number of words or characters in a review | Numerical | Examine review characteristics |
| Mentioned Attributes | Product aspects discussed, such as fragrance or packaging | Text/Categorical | Identify common likes and complaints |

Some variables, including sentiment, review length, and mentioned attributes, may need to be derived during preprocessing rather than obtained directly from the original dataset.

## 4. Data Requirements

The selected dataset should ideally meet the following requirements:

1. Contain review text and associated product ratings.
2. Focus on beauty, skincare, makeup, haircare, or related personal-care products.
3. Provide enough usable records to support descriptive analysis.
4. Include product identifiers or names for product-level comparisons.
5. Provide clear source information and documentation.
6. Be publicly accessible under terms that permit the intended research use.
7. Have manageable missing values and duplication issues.
8. Include dates or categories where available for additional analysis.

The exact dataset size and available columns will be confirmed during Week 2.

## 5. Data Types and Their Uses

### Numerical Data
Examples include product ratings and review length. These variables support summary statistics, distributions, and comparisons.

### Categorical Data
Examples include product category and sentiment class. These variables support frequency tables and group comparisons.

### Text Data
Examples include review titles and review text. These are essential for NLP, sentiment classification, and identifying recurring topics.

### Date/Time Data
Review dates can help examine changes in ratings and sentiment over time if the dataset has sufficient temporal coverage.

## 6. Derived Variables

The following variables may be created from the original data:

- **Sentiment Label:** Predicted or assigned sentiment based on review text.
- **Review Length:** Number of words or characters in a review.
- **Rating Group:** Grouped ratings, such as low, medium, and high, where appropriate.
- **Mentioned Product Attributes:** Themes such as price, quality, fragrance, texture, packaging, and effectiveness.
- **Review Period:** Month, quarter, or year extracted from the review date.

Any sentiment labels derived from ratings must be distinguished from labels predicted from review text to avoid circular evaluation.

## 7. Data Quality Considerations

The following issues will be checked:

- Missing review text, ratings, or product identifiers.
- Duplicate reviews and repeated records.
- Invalid ratings or inconsistent rating scales.
- Very short, irrelevant, or non-informative reviews.
- HTML tags, emojis, unusual characters, and spelling variations.
- Different languages or mixed-language reviews.
- Uneven numbers of positive and negative reviews.
- Potentially misleading or biased reviews.

Records will not be removed automatically. Cleaning decisions will depend on the dataset, analysis goals, and documented criteria.

## 8. Data Privacy and Responsible Use

Only data that can be accessed and used under the applicable dataset terms will be considered. Personal identifiers will not be required for the core sentiment analysis and will be excluded or anonymized where appropriate. The analysis will focus on aggregate customer feedback rather than identifying individual reviewers.

## 9. Conclusion

Defining the required variables and data quality criteria provides a clear foundation for data collection and exploratory analysis. The final variable list will be adjusted to match the columns available in the selected public dataset.

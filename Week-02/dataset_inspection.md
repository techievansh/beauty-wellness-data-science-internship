# Dataset Inspection Report

## 1. Project Title
Customer Sentiment Analysis of Beauty Product Reviews

## 2. Dataset Source
Amazon Beauty Reviews Dataset

Platform: Hugging Face

Link: https://huggingface.co/datasets/jhan21/amazon-beauty-reviews-dataset

## 3. Purpose of Inspection
The purpose of dataset inspection is to understand the dataset structure, identify important columns, and assess its suitability for customer sentiment analysis.

## 4. Observed Columns

The dataset preview contains the following columns:

- rating: Numerical customer rating.
- title: Review headline.
- text: Detailed customer review.
- images: Image information associated with a review.
- asin: Product identifier.
- parent_asin: Parent product identifier.
- user_id: Reviewer identifier.
- timestamp: Review date and time.
- helpful_vote: Number of helpful votes.
- verified_purchase: Indicates whether a purchase was verified.

## 5. Initial Observations

The displayed sample records contain ratings from 1 to 5 and review text of varying lengths. Some reviews describe positive experiences, while others mention problems such as product smell, quality, or usability.

The verified_purchase field contains Boolean values, and helpful_vote records the number of helpful votes. Some reviews contain image information, while others have empty image lists.

## 6. Data Quality Considerations

The following checks are required before analysis:

- Missing and empty review text.
- Duplicate reviews.
- Invalid or out-of-range ratings.
- Missing titles and product identifiers.
- Timestamp parsing and date consistency.
- Distribution of ratings and verified purchases.
- Reviews that are irrelevant or contain insufficient information.

## 7. Suitability for Sentiment Analysis

The rating and text columns are particularly useful. Review text can be analyzed using natural language processing, while ratings can provide an initial reference for positive and negative sentiment. Neutral sentiment must be defined carefully, and rating-based labels should not be treated as perfect representations of sentiment.

## 8. Limitations

The preview alone does not establish the overall data quality, missing-value percentage, rating distribution, or duplicate count. These must be measured using a sample or the full dataset. The dataset license and usage conditions must also be verified.

## 9. Conclusion

The inspected sample indicates that the dataset has relevant fields for beauty-product review analysis. Further quantitative checks are necessary before preprocessing, visualization, and sentiment classification begin.

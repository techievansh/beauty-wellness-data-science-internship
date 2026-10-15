# Data Sourcing Strategy

## 1. Project Title
Customer Sentiment Analysis of Beauty Product Reviews

## 2. Objective
The objective is to establish a structured strategy for identifying, accessing, collecting, and preparing relevant data for customer sentiment analysis in the beauty and wellness industry.

## 3. Primary Data Source
**Dataset:** Amazon Beauty Reviews Dataset

**Platform:** Hugging Face

**Link:** https://huggingface.co/datasets/jhan21/amazon-beauty-reviews-dataset

This dataset is the preliminary choice because its preview includes customer ratings, review text, review titles, timestamps, helpful votes, and verified purchase indicators.

The dataset's suitability will be confirmed after checking its structure, quality, licensing, and access conditions.

## 4. Backup Data Sources

1. **Sephora Products and Skincare Reviews:** https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews
2. **Sephora Skincare Reviews and Sentiment:** https://huggingface.co/datasets/haoxianc/natashamessier_sephora-skincare-reviews-and-sentiment

These sources may be used if the primary dataset does not meet the project's requirements. Their fields, accessibility, and usage permissions must be checked before use.

## 5. Data Collection Method
The proposed collection process is:

1. Open the dataset's official hosting page.
2. Review the dataset description, available files, columns, and access instructions.
3. Check the licence and permitted usage.
4. Load a manageable sample using an appropriate supported method.
5. Inspect the sample to confirm that the required fields are available.
6. Record any access issues and data limitations.
7. Save the dataset reference and document the collection method.

The complete dataset will not be downloaded unnecessarily during the initial inspection stage.

## 6. Key Variables Required

- **Rating:** Numerical customer rating.
- **Review Text:** Written feedback used for text analysis.
- **Review Title:** Optional review summary.
- **Timestamp:** Review date, if available.
- **Helpful Votes:** Number of helpful votes, if available.
- **Verified Purchase:** Purchase verification indicator, if available.
- **Product Identifier:** Identifier used to associate reviews with products.

## 7. Data Quality and Reliability
The following checks will be planned before analysis:

- Missing or empty review text.
- Duplicate reviews.
- Ratings outside the expected range.
- Missing product identifiers.
- Invalid or inconsistent timestamps.
- Unusually short, irrelevant, or low-information reviews.
- Potentially misleading or inconsistent sentiment labels.

The presence and extent of these issues will be determined through actual inspection rather than assumed in advance.

## 8. Accessibility and Usage Permissions
The availability of a public dataset does not automatically mean unrestricted use. Its licence, attribution requirements, redistribution conditions, and any applicable platform restrictions must be reviewed.

If an API is considered, its authentication requirements, rate limits, cost, and permitted uses must also be checked. Restricted or private customer information will not be intentionally collected.

## 9. Data Storage and Documentation
The project will maintain a record of the dataset name, source link, access date, relevant columns, collection method, licence information, and known limitations.

Only the data required for the project will be collected. Any generated analysis files will be organised in the project repository, subject to the dataset's redistribution conditions.

## 10. Conclusion
A structured sourcing strategy has been established for the beauty product sentiment analysis project. The Amazon Beauty Reviews dataset is the initial candidate, with Sephora review datasets as alternatives. Final selection will depend on verified accessibility, data quality, relevance, and usage permissions.

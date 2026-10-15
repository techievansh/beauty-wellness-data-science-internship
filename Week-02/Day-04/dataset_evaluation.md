# Dataset Evaluation and Selection

## 1. Project Title
Customer Sentiment Analysis of Beauty Product Reviews

## 2. Objective
The objective is to evaluate potential datasets and identify the most suitable source for analysing customer sentiment in beauty product reviews.

## 3. Evaluation Criteria
The following criteria will be used:

- **Relevance:** Whether the dataset contains beauty product reviews and customer opinions.
- **Accessibility:** Whether the data can be accessed through its hosting platform.
- **Completeness:** Whether important fields such as ratings and review text are available.
- **Data Quality:** Whether the dataset can be checked for missing values, duplicates, and invalid records.
- **Format:** Whether the data can be processed using Python and common data analysis tools.
- **Usage Permissions:** Whether the dataset's licence and conditions permit the intended analysis.

## 4. Candidate Dataset 1: Amazon Beauty Reviews

**Link:** https://huggingface.co/datasets/jhan21/amazon-beauty-reviews-dataset

**Advantages:**
- The inspected preview contains customer ratings and written reviews.
- Additional fields include review titles, timestamps, helpful votes, and verified purchase indicators.
- The available fields appear relevant to exploratory data analysis and sentiment research.

**Limitations:**
- The full dataset's completeness and quality have not yet been measured.
- Duplicate records and missing values need to be checked.
- Licensing and permitted usage must be verified.

**Preliminary assessment:** Strong initial candidate because the inspected sample contains relevant review and rating fields.

## 5. Candidate Dataset 2: Sephora Products and Skincare Reviews

**Link:** https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews

**Advantages:**
- Focuses on beauty products and skincare.
- May provide product information alongside reviews.
- Offers an alternative for comparing product-specific feedback.

**Limitations:**
- Access may require a Kaggle account.
- The exact structure and completeness need verification.
- Licence and update frequency must be checked.

**Preliminary assessment:** A relevant backup candidate, subject to further inspection.

## 6. Candidate Dataset 3: Sephora Skincare Reviews and Sentiment

**Link:** https://huggingface.co/datasets/haoxianc/natashamessier_sephora-skincare-reviews-and-sentiment

**Advantages:**
- Focuses on skincare reviews and sentiment-related information.
- May provide an alternative for examining sentiment labels.
- Could support comparison with rating-based sentiment.

**Limitations:**
- The available columns and label-generation method require verification.
- Existing labels may not always represent the meaning of review text accurately.
- Licensing and dataset coverage need to be checked.

**Preliminary assessment:** A potential alternative if its structure and labels meet project requirements.

## 7. Comparative Evaluation

| Criterion | Amazon Beauty Reviews | Sephora Kaggle | Sephora Sentiment |
|---|---|---|---|
| Industry relevance | High | High | High |
| Review text availability | Observed in preview | Verify | Verify |
| Rating availability | Observed in preview | Verify | Verify |
| Accessibility | Public hosting page | Account may be required | Public hosting page |
| Data quality | Requires measurement | Requires inspection | Requires inspection |
| Usage permissions | Verify licence | Verify licence | Verify licence |

The comparison is preliminary. Ratings such as high relevance reflect the dataset descriptions and inspected preview, not a completed quantitative quality audit.

## 8. Selected Dataset
The Amazon Beauty Reviews dataset is the preliminary selection because the inspected preview contains review text, numerical ratings, and several useful supporting fields.

Before final confirmation, the dataset's licence, data quality, and suitability for the intended analysis must be verified.

## 9. Risks and Limitations
Potential risks include missing data, duplicate reviews, unrepresentative samples, biased customer feedback, and differences between star ratings and written sentiment. These risks will be assessed during the data inspection and preprocessing stages.

## 10. Conclusion
The three candidate datasets have been considered against relevance, accessibility, completeness, data quality, and usage requirements. Amazon Beauty Reviews is the initial choice, while the Sephora datasets remain alternatives pending verification.

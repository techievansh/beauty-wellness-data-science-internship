# Initial Exploratory Data Analysis Plan

## 1. Project Title
Customer Sentiment Analysis of Beauty Product Reviews

## 2. Objective
The objective is to develop a preliminary exploratory data analysis (EDA) plan for understanding customer ratings, review text, review characteristics, and data quality in beauty product reviews.

## 3. Key Variables

| Variable | Type | Planned Analysis |
|---|---|---|
| rating | Numerical or ordinal | Rating frequency and distribution |
| text | Text | Review length, common words, and sentiment exploration |
| title | Text | Headline patterns and additional context |
| timestamp | Date/time | Review trends over time, if suitable |
| helpful_vote | Numerical count | Distribution and outlier inspection |
| verified_purchase | Boolean | Comparison of verified and unverified reviews |
| asin | Identifier | Product-level grouping where useful |

The availability, completeness, and meaning of each field will be verified before analysis.

## 4. Data Quality Assessment
The first stage will assess:

- Missing and empty values.
- Duplicate records and repeated review text.
- Invalid rating values.
- Review text quality and length.
- Timestamp validity and consistency.
- Outliers in helpful-vote counts.
- The number of verified and unverified purchases.

The results will be recorded using actual counts and percentages once the data is loaded.

## 5. Descriptive Statistics
The following statistics are planned:

- Total number of reviews analysed.
- Mean, median, minimum, and maximum rating.
- Frequency and percentage of each rating value.
- Missing-value counts and percentages.
- Average and median review length.
- Distribution of helpful votes.
- Proportion of verified purchases.
- Review counts over time, if timestamps are suitable.

Median and frequency-based summaries will be included because ratings and helpful-vote counts may not follow a normal distribution.

## 6. Planned Visualisations

### Rating Distribution
A bar chart will show the number of reviews for each rating.

### Review Length Distribution
A histogram will show the distribution of review lengths.

### Rating and Review Length
A box plot may compare review lengths across rating groups.

### Helpful Votes
A histogram or box plot will help examine the distribution and potential outliers of helpful votes.

### Verified Purchase Comparison
A grouped bar chart will compare rating distributions for verified and unverified purchases.

### Review Trends
A line chart may show the number of reviews over time if the timestamps provide sufficient reliable coverage.

### Common Review Terms
A bar chart of frequent terms or a word cloud may help explore language patterns. Common words should be interpreted in context rather than treated as proof of sentiment.

## 7. Statistical Methods
- Frequency tables and percentages for categorical and ordinal values.
- Mean, median, standard deviation, and quartiles for suitable numerical variables.
- Group comparisons to explore differences between rating categories.
- Correlation analysis between suitable numerical variables, with caution when interpreting ordinal ratings.
- Optional statistical tests after checking assumptions and defining the research question.

Exploratory associations will not automatically be interpreted as causal relationships.

## 8. Text Preprocessing Plan
The following steps may be applied to review text:

1. Remove missing or empty reviews where appropriate.
2. Standardise unnecessary whitespace.
3. Handle unusual characters and encoding issues.
4. Convert text to a consistent case when appropriate.
5. Tokenise text for word-level analysis.
6. Consider stop-word removal for selected analyses.
7. Preserve negation words such as "not" when analysing sentiment.
8. Review repeated text and duplicates before removing records.

Preprocessing choices will depend on the intended analysis and should not remove meaningful customer information.

## 9. Hypothesis Testing Plan
- **H1:** Compare review language across high and low rating groups.
- **H2:** Examine the frequency and themes of complaints in lower-rated reviews.
- **H3:** Compare review-length distributions across rating groups.
- **H4:** Explore how helpful votes vary with rating and review length.

These analyses will provide evidence for evaluating the hypotheses. Findings will be reported only after the analysis has been performed.

## 10. Tools
- Python for data analysis.
- Google Colab for notebook-based work.
- Pandas for data manipulation.
- Matplotlib and Seaborn for visualisations.
- Suitable text-processing libraries for later sentiment exploration.

## 11. Expected Outcome
The planned EDA should provide a clearer understanding of rating patterns, review text, data quality, and relationships between selected variables. It will also help determine whether the dataset is ready for further sentiment analysis.

## 12. Limitations
The analysis may be affected by biased customer participation, missing information, repeated reviews, and differences between written sentiment and star ratings. These limitations will be considered when interpreting results.

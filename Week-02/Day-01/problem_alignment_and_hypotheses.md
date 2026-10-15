# Problem Alignment and Hypotheses

## 1. Project Title
Customer Sentiment Analysis of Beauty Product Reviews

## 2. Industry Overview
The beauty and wellness industry includes skincare, haircare, cosmetics, and personal care products. Customers frequently share their experiences through online reviews and ratings. Analysing these reviews can help businesses understand customer satisfaction, product quality concerns, and consumer preferences.

## 3. Problem Statement
Beauty product businesses receive a large number of online customer reviews. Manually reading and analysing every review can be time-consuming. This makes it difficult to identify common complaints, understand customer opinions, and recognise areas for product improvement.

This project aims to explore customer sentiment in beauty product reviews using review text and star ratings. The analysis will help identify positive and negative feedback and assess the suitability of the data for future sentiment classification.

## 4. Project Objectives
- Analyse customer reviews of beauty products.
- Examine the distribution of customer ratings.
- Identify common positive feedback and negative complaints.
- Explore the relationship between review text and star ratings.
- Plan initial exploratory data analysis.
- Assess whether the selected dataset is suitable for sentiment analysis.

## 5. Research Questions
1. What is the distribution of customer ratings?
2. What themes commonly appear in positive and negative reviews?
3. Do written reviews generally agree with their star ratings?
4. Which product-related concerns appear frequently in negative reviews?
5. What data quality issues may affect the analysis?

## 6. Initial Hypotheses

**H1: Rating and Sentiment**

Reviews with higher star ratings are expected to contain more positive language than reviews with lower star ratings.

**H2: Negative Reviews and Complaints**

Lower-rated reviews are expected to contain more complaints about product quality, usability, smell, or customer experience.

**H3: Review Length and Rating**

Review length may vary across different rating groups.

**H4: Helpful Votes and Review Characteristics**

The number of helpful votes may vary depending on review length, rating, and the usefulness of the information provided.

These hypotheses will be investigated during the analysis. They are expectations to test, not confirmed findings.

## 7. Required Data Fields
- **Rating:** The numerical star rating given by the customer.
- **Review Text:** The written description of the customer's experience.
- **Review Title:** A short summary or headline of the review.
- **Timestamp:** The date and time when the review was submitted.
- **Helpful Votes:** The number of votes indicating that a review was helpful.
- **Verified Purchase:** Indicates whether the purchase was verified.
- **Product Identifier:** Identifies the product associated with a review.

The availability and completeness of these fields must be checked before analysis.

## 8. Proposed Approach
The project will use a publicly available beauty product review dataset. Initial analysis will include examining ratings, reviewing sample text, checking data quality, and identifying common words or themes.

Rating-based sentiment labels may be explored as an initial approximation, but star ratings will not be treated as perfect representations of sentiment. Some reviews may contain mixed opinions or text that does not match the rating.

## 9. Expected Outcome
The initial work is expected to establish a clear problem definition, identify relevant data requirements, and provide testable hypotheses. It will also guide dataset selection, preprocessing, exploratory analysis, and future sentiment classification.

## 10. Scope and Limitations
This stage focuses on problem definition and analysis planning. It does not establish that any hypothesis is true. Results will depend on the quality, representativeness, completeness, and permitted use of the selected dataset.

The analysis of online reviews may not represent every beauty product customer, and findings should be interpreted within the limits of the available data.

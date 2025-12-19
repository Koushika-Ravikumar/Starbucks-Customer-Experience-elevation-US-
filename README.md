# Analyzing Starbucks Customer Experience in the US

This project analyzes Starbucks customer experience in the United States using transactional and survey-style data to understand how store attributes, product choices, and customer behavior relate to satisfaction and repeat visits.

## Project Overview

The analysis combines exploratory data analysis (EDA) and modeling in Python to evaluate key drivers of customer experience at Starbucks stores across the US.  
Findings are summarized in an executive presentation and grounded in a written proposal that defines the business context and objectives.

## Files in this Repository

- `starbucks_data.csv` – Raw dataset containing customer-, store-, and transaction-level information used for the analysis.
- `ProjectEDA.ipynb` / `ProjectEDA.html` – Exploratory data analysis notebook and HTML export with data cleaning, feature exploration, and visualization. 
- `Final-code.ipynb` / `Final-code.html` – Final modeling and analysis notebook plus HTML report (e.g., feature engineering, model training, evaluation, and insights).
- `CIS509-Starbucks-review.pptx` – Slide deck summarizing key findings, visualizations, and recommendations for stakeholders.  
- `Proposal-submission.pdf` – Initial project proposal describing background, motivation, research questions, and planned methodology.

## Objectives

- Quantify how different factors (store location, visit frequency, product mix, spend, etc.) impact customer experience metrics such as satisfaction and loyalty.
- Identify segments of Starbucks customers in the US with distinct behaviors and preferences.  
- Generate actionable recommendations for improving customer experience and retention at Starbucks stores based on data-driven evidence.

## Methods

Our analysis follows a text‑analytics and sentiment‑driven pipeline built on Yelp business and review data for Starbucks locations across the US.

- **Data collection & integration**
  - Collect Yelp business and review JSON files for coffee and café businesses in the US.
  - Inner‑join business and review data, then filter to Starbucks locations only (≈20,000 reviews from an initial ≈60,000+ records).

- **Data preprocessing & cleaning**
  - Remove spam, duplicates, and records with missing or unusable fields.
  - Keep only relevant categories (coffee / café) and Starbucks businesses.

- **Sentiment analysis**
  - Compute sentiment scores for each review text and pair them with star ratings.
  - Analyze average sentiment and review scores over time and by state (e.g., Delaware, Idaho, Arizona, Missouri, Louisiana).  
  - Study trends from 2008–2022 to identify states with declining or improving customer sentiment.

- **Correlation analysis**
  - Build a correlation matrix between star ratings (`stars_x`) and sentiment scores (`sentiment`).
  - Find a correlation of about 0.65, showing that more positive sentiment generally aligns with higher star ratings while leaving room for other factors such as price, service quality, and expectations.

- **Geographic & keyword analysis (TF‑IDF)**
  - Use TF‑IDF vectorization on review text to surface important keywords in high‑ and low‑rated reviews across regions.
  - Compare positive language (e.g., friendly, great, love, nice) versus negative patterns (e.g., line, minutes, ordered, asked) to understand drivers of satisfaction and complaints.

- **Managerial recommendations**
  - Identify high‑performing markets (AZ, MO, LA) and compare their cleaning, parking, and operational practices to lower‑performing states.
  - Recommend sharing best practices via manager meetings and support teams, and continuously monitoring Yelp scores and sentiment to evaluate policy impact.

## Potential Use Cases

- **Customer Analytics / Data Science roles** – Demonstrates end-to-end work from proposal to EDA, modeling, and stakeholder storytelling.  
- **Retail & CPG analytics** – Relevant for roles focused on store performance, customer experience, CRM, and loyalty programs.


## Overview
This project focuses on extracting actionable insights from Trustpilot reviews for a Lebara, using customer feedback stored in Databricks, we perform sentiment analysis, keyword extraction and RAG to identify areas of improvement and key strengths. The data is enriched with metrics such as Churn Score, Average Customer Value, Tenure, Last Usage Date and Customer Type. This data is fed into Power BI dashboards and reports and can be used to take proactive actions to improve customer satisfaction rating.

## Sentiment Analysis:
•	We use a Hugging Face pre-trained model for sentiment analysis to classify reviews into:
- o	Positive
- o	Neutral
- o	Negative
•	Confidence scores are utilized to fine-tune the classification, ensuring neutral sentiments are accurately captured.

## Keyword Extraction:
-  •	KeyBERT is utilized to extract keywords from the review text.
-  •	This helps in identifying recurring themes, pain points, and strengths for better decision-making.

## RAG (Retrieval Augmented Generation using databricks)
Using d**atabricks-gte-large-en** – created vector database and for langchain we have used **databricks-meta-llama-3-1-70b-instruct** model to create interactive bot

## Data Enrichment:
Data is linked to existing subscribers and enhanced to include there churn score, country, customer type and last usage date

## Technologies Used
### Infrastructure

**•	Databricks:**
o	Used for data storage (Delta Lake) and processing.
o	Provides scalable computation for handling large datasets.

**Libraries and Tools**
- •	Hugging Face Transformers: For sentiment analysis using pre-trained NLP models.
- •	KeyBERT: For extracting keywords from text using BERT embeddings.
- •	PySpark: For distributed processing of large-scale reviews.
- •	Delta Lake: For efficient and scalable data storage.
- •	Pandas – for data analysis
- •	RAG - for auto reply 

## Outputs
### •	Sentiment Analysis Results:
  Reviews Classified As : Positive , Negative and Neutral ,   Sentment scoring
  

### •	Keyword Insights:
  Frequent terms associated with positive and negative reviews ,  Categorized themes for actionable insights.
   

### •	Automated reply / custom bot for actionable insights
  User can directly type in questions and get the feed back 
    
### •	Trends and Metrics:
Distribution of sentiments over time.  Most common keywords and recurring issues.   High value customers with negative review
 .




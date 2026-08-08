# -Ola-vs.-Uber-Google-Play-Store-Sentiment-Customer-Experience-Analysis
🚗 Ola vs. Uber: Sentiment &amp; Experience Analysis — NLP project on Google Play reviews comparing Ola &amp; Uber. Uses VADER with Hinglish lexicon to quantify sentiment, extract pain points (driver issues, cancellations, pricing, app bugs), and visualize trends. Uber shows higher positivity, Ola faces more negatives

📌 Project Overview
Ride-hailing platforms rely heavily on customer satisfaction and feedback loops. This notebook conducts an end-to-end exploratory data analysis (EDA) and sentiment analysis on Play Store reviews for Ola and Uber to answer key strategic questions:

How do user sentiments compare across both platforms?

What are the major operational and app-level pain points (e.g., driver behavior, cancellations, pricing, app bugs)?

How do developer responses impact user ratings and satisfaction?

What key features and improvements do users request most frequently?

# ✨ Key Features & Methodology
Data Scraping & Preprocessing:

Leveraged google_play_scraper to extract raw review data (ratings, review text, dates, developer responses, app versions).

Cleaned text data by lowercasing, removing special characters/URLs, and handling repeated characters.

Custom Hinglish Sentiment Analysis:

Customized NLTK's vaderSentiment analyzer with a dedicated Hinglish lexicon (e.g., bakwas, bekar, ghatiya, badhiya, badiya, mast) to accurately capture sentiment in Indian colloquial English/Hindi reviews.

Pain Point & Priority Scoring:

Categorized negative user feedback into core themes: Driver Issues, Cancellations, Customer Support, App Issues, Payment Issues, and High Pricing.

Calculated a custom Priority Score combining review frequency, sentiment intensity, and rating impact to pinpoint critical focus areas for product teams.

Visualizations & Insights:

Interactive Plotly charts for overall sentiment comparison.

Keyword extraction and Matplotlib/Seaborn rating distribution trends over time.

Side-by-side Word Cloud generation for Ola vs. Uber.

# 📊 Key Findings
Overall Sentiment: Uber exhibits a significantly higher positive review percentage (~66.8%) compared to Ola (~41.6%), while Ola faces a higher negative sentiment proportion (~46.1%).

Primary Pain Points: Driver behavior and ride cancellations emerged as the highest priority pain points for both services.

Developer Engagement: Analyzed developer response rates and their correlation with user ratings and review sentiment over time.



Natural Language Processing (NLP): vaderSentiment, nltk, transformers (Hugging Face), torch

Data Visualization: matplotlib, seaborn, plotly, wordcloud

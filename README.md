# Real-Time-Reddit-Sentiment-Viz

This project aims to fetch trending news articles, analyze public sentiment on Reddit discussions related to those articles, and visualize insights using Power BI dashboards. The goal is to try and understand public sentiment trends to support targeted marketing strategies and audience engagement.

# How It Works
1) Fetch News Titles: Use the News API to gather titles of trending news articles across selected categories.

2) Analyze Reddit Sentiment:
    - Search Reddit for posts matching the news topics.
    - Collect comments from the posts and calculate sentiment scores using NLTK's SentimentIntensityAnalyzer.

3) Stream Data to Azure:
    - Send processed data (news titles, Reddit post titles, comment sentiment scores) to Azure Event Hubs.
    - Process Data with Azure Stream Analytics:
    - Route data to Power BI for visualization.
    - Store data in Azure Blob Storage for historical analysis.

4) Visualize Insights: Display real-time dashboards in Power BI to track sentiment trends and popular topics.

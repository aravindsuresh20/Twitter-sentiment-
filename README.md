🐦 twitter.py — Twitter Sentiment Analysis Dashboard
Purpose:
Analyzes sentiment in tweets from a CSV file using TextBlob and applies conditional formatting in Excel for easy visualization.

🔧 Features & Workflow
📥 Load Dataset

Reads data from:
D:/twitter new sentiment/twitter_dataset.csv
🧹 Preprocessing

Strips whitespace from column names.
Uses the Text column for sentiment analysis.
💬 Sentiment Analysis

Uses TextBlob to compute:
Sentiment: 'Positive', 'Negative', or 'Neutral'
Sentiment_Percentage: magnitude of polarity × 100
Sentiment_Score: raw polarity score
📊 Output

Saves results to:
D:/twitter new sentiment/twitter_dataset_colored.xlsx
🎨 Excel Formatting

Applies color coding to the Sentiment column:
✅ Green for Positive
⚠️ Yellow for Negative
Neutral remains uncolored

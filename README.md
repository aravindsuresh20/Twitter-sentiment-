Markdown

# Twitter Sentiment Analysis with Python and TextBlob

This project provides a Python script (`twitter.py`) designed to perform sentiment analysis on Twitter data from a CSV file. It leverages the `TextBlob` library for sentiment calculation and `pandas` for data manipulation. The script processes the 'Text' column of your dataset, categorizes each tweet's sentiment (Positive, Negative, Neutral), calculates sentiment percentage and a numerical score, and then saves the results to an Excel file. For better visualization, it applies conditional formatting to the output Excel, highlighting 'Positive' and 'Negative' sentiments with distinct background colors.

## Features

* **CSV Data Loading:** Reads tweet data from a specified CSV file.
* **Sentiment Analysis:** Utilizes `TextBlob` to determine the sentiment (Positive, Negative, Neutral) of each tweet.
* **Sentiment Metrics:** Calculates a sentiment percentage and a numerical sentiment score for each tweet.
* **Excel Export:** Saves the original data along with the new sentiment columns to an Excel file (`.xlsx`).
* **Conditional Formatting:** Automatically colors 'Positive' sentiment cells in green and 'Negative' sentiment cells in yellow within the output Excel file for quick visual insights.

## Requirements

Ensure you have the following Python libraries installed. You can install them using `pip`:

```bash
pip install pandas textblob openpyxl
Additionally, TextBlob requires its corpora to be downloaded for full functionality:

Bash

python -m textblob.download_corpora
Installation
Save the Script: Download or copy the twitter.py script into your desired project directory.

Prepare Your Data: Place your Twitter dataset in a CSV file (e.g., twitter_dataset.csv) in the same directory as the twitter.py script, or update the input_file variable in twitter.py to the full path of your CSV. Ensure your CSV has a column named Text containing the tweet content.

Virtual Environment (Recommended):
It's good practice to set up a virtual environment to manage dependencies:

Bash

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Usage
Run the Script: Open your terminal or command prompt, navigate to the directory where you saved twitter.py and your CSV, and execute the script:

Bash

python twitter.py
Output File: Upon successful execution, a new Excel file named twitter_dataset_colored.xlsx (or as specified in the output_file variable within twitter.py) will be generated in the same directory. This file will contain the original tweet data, along with new columns for 'Sentiment', 'Sentiment_Percentage', and 'Sentiment_Score', with sentiment cells conditionally colored.

Review Results: Open the twitter_dataset_colored.xlsx file using Microsoft Excel or a compatible spreadsheet program to view the sentiment analysis results and the applied conditional formatting.

Project Structure
/your-project-directory/
│── twitter.py                # Main script for sentiment analysis
│── twitter_dataset.csv       # Example input Twitter dataset
│── twitter_dataset_colored.xlsx # Output Excel file with sentiment results
│── README.md                 # This documentation file

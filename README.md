Twitter Sentiment Analysis
This project provides a Python script to perform sentiment analysis on a Twitter dataset stored in a CSV file. It uses the TextBlob library to analyze the sentiment of tweet texts and then saves the results, including sentiment classification, sentiment percentage, and sentiment score, to an Excel file. Positive and Negative sentiments are highlighted with different background colors in the Excel output.

Features
Loads tweet data from a CSV file.

Performs sentiment analysis (Positive, Negative, Neutral) on the 'Text' column.

Calculates sentiment percentage and a numerical sentiment score.

Saves the processed data to an Excel file.

Applies conditional formatting in the Excel file:

Green background for 'Positive' sentiments.

Yellow background for 'Negative' sentiments.

Requirements
Ensure you have the following Python libraries installed:

pandas

textblob

openpyxl

You can install them using pip:

Bash

pip install pandas textblob openpyxl
You might also need to download the TextBlob data after installing it:

Bash

python -m textblob.download_corpora
Installation
Save the twitter.py file:
Ensure the twitter.py script is saved in your desired working directory.

Set up a virtual environment (optional but recommended):

Bash

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Usage
Prepare your dataset:
Ensure your Twitter data is in a CSV file named twitter_dataset.csv (or update the input_file variable in twitter.py to your file path). The CSV file must contain a column named Text with the tweet content.

Run the script:

Bash

python twitter.py
Check the output:
A new Excel file named twitter_dataset_colored.xlsx will be generated in the same directory as your input CSV file (or the path specified in output_file in twitter.py). This file will contain the original data along with the new 'Sentiment', 'Sentiment_Percentage', and 'Sentiment_Score' columns, with sentiment cells colored accordingly.

Project Structure
/your-project-directory
│── twitter.py           # Main Python script for sentiment analysis
│── twitter_dataset.csv  # Input Twitter dataset (example)
│── twitter_dataset_colored.xlsx # Output Excel file
│── README.md            # Project documentation

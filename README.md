# TOI News Analysis using Top2Vec

This project demonstrates how to collect news data from the Times of India (TOI) website, perform topic modeling using Top2Vec, and visualize the results using word clouds and a Louvain community chart.

## Steps

1. **Data Collection:**
   - Scrape news articles from the TOI website for selected cities (Hyderabad, Bangalore, Chennai, Mumbai, Delhi, Pune, Kolkata).
   - Store the collected text data in a CSV file.

2. **Data Preprocessing:**
   - Load the news data from the CSV file.
   - Remove empty strings and stop words from the text.

3. **Top2Vec Modeling:**
   - Create a Top2Vec model using the preprocessed news articles.
   - Use the Universal Sentence Encoder for embedding generation.

4. **Topic Visualization:**
   - Generate word clouds for each topic identified by the Top2Vec model.
   - Create a Louvain community chart to visualize the relationships between topics.

## Requirements

- Python 3
- Libraries: requests, bs4, pandas, top2vec, nltk, wordcloud, matplotlib, networkx, python-louvain

## Installation

1. Install the required libraries:
   - bash pip install requests bs4 pandas top2vec[sentence_encoders] wordcloud matplotlib networkx python-louvain
2. Download NLTK stopwords:
   - python import nltk nltk.download('stopwords')
## Usage

1. Run the provided Jupyter Notebook code to perform web scraping, topic modeling, and visualization.
2. Adjust the `LIST_OF_CITIES` and `PAGINATION_UPTO` variables to customize the data collection process.
3. Modify the `threshold` value in the Louvain community detection section to control the granularity of topic clusters.

## Disclaimer

This project is for educational purposes only. Web scraping should be conducted responsibly and in accordance with the website's terms of service.

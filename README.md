# Multilingual-Movie-Review-Sentiment-Analysis-with-Transformers

## Project Overview
This project aims to analyze the sentiment of movie reviews written in three different languages: English, French, and Spanish. The reviews and synopses for 30 movies (10 in each language) are provided in CSV files. The primary objectives are to translate non-English reviews to English and perform sentiment analysis on all reviews.

## Dataset
The dataset includes three CSV files:

* movie_reviews_eng.csv - English reviews and synopses
* movie_reviews_fr.csv - French reviews and synopses
* movie_reviews_sp.csv - Spanish reviews and synopses
* Each file contains the following columns: Title, Year, Synopsis, and Review.

## Steps Involved
### Data Preparation:
* Load all CSV files and merge them into a single Pandas DataFrame.
* Add a column Original Language to track the language of each review.

### Translation:
* Translate French and Spanish reviews and synopses to English using pre-trained models from HuggingFace Transformers.
  
### Sentiment Analysis:
* Analyze the sentiment of each review (Positive or Negative) using a pre-trained sentiment analysis model from HuggingFace.
* Add a Sentiment column to the DataFrame with the results.

### Output:
* Export the final DataFrame to a CSV file, containing the columns: Title, Year, Synopsis, Review, Sentiment, and Original Language.


## Tools Used
* Pandas: For data manipulation and analysis.
* HuggingFace Transformers: For natural language processing tasks, including translation and sentiment analysis.
* PyTorch: For utilizing the machine learning models.

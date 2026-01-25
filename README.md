# Serbian News Channel Analysis from Nov 1st 2024 to January 2026

## Files structure
1. Data - csv fils containing news articles
   - n1.csv - all of the collected articles from N1 news channel (34673 articles)
   - rts.csv - all of the collected articles from RTS news channel (3367 articles)
   - n1_cleaned - deleted duplicates and articles before 31st October 2024 (around 34673 articles)
   - n1_cleaned_with_scores - dataset with results after applying a model to determine if articles are related or unrelated to the protests (around 34000 articles)
   - rts_latin - cleaned articles from RTS with data in Serbian latin script instead of Serbian cyrilics
   - random_headlines.csv - 570 randomly sampled headlines from n1 dataset that I manually labeled as related and undrelated to the protests for validation
2. Code - contains code used for the analysis
   - News_Data_Scraping.ipynb - includes the code used for web scraping both websites
   - Data_Cleaning.ipynb - includes the code used for cleaning the datasets
3. Test - contains code used for trying out different functions


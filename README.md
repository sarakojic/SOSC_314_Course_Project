# Serbian News Channel Analysis from Nov 1st 2024 to January 2026

## Files structure
1. Data - csv fils containing news articles
   - n1.csv - all of the collected articles from N1 news channel (39000 articles)
   - rts.csv - all of the collected articles from RTS news channel (3400 articles)
   - n1_cleaned - deleted duplicates and articles before 31st October 2024
   - n1_cleaned_with_scores - dataset with results after applying a model to determine if articles are related or unrelated to the protests
2. Code - contains code used for the analysis
   - News_Data_Scraping.ipynb - includes the code used for web scraping both websites
   - Data_Cleaning.ipynb - includes the code used for cleaning the datasets
3. Test - contains code used for trying out different functions


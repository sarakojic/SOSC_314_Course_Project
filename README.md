# Serbian News Channel Analysis from Nov 1st 2024 to January 2026
## Problem setup
The goal of this projet is to analyze the way in which two different news chnannnels in Serbia report on the protests.

The two news channnels chosen for comparison are N1 [https://n1info.rs/] and RTS [https://www.rts.rs/lat.html?print=true].

The reason I chose these two news channels specifically is because N1 is usually considered as the only independent news source in Serbia, while RTS is a government-ran news channel

### Project tasks
1. analyze common words used by RTS and N1
2. compare the frequency of the published articles related to the protest over months
3. analyze different event types and their occurances over months in the news articles published by RTS and N1


## Files structure
1. data - csv fils containing news articles
   - https://duke.box.com/s/inv45b53h9czkrgjto91ath2ifx2manm link to access the dataset containing full text of n1 articles
   - n1.csv - all of the collected articles from N1 news channel (34673 articles)
   - rts.csv - all of the collected articles from RTS news channel (3367 articles)
   - n1_cleaned_with_scores - dataset with results after applying a model to determine if articles are related or unrelated to the protests (around 34000 articles)
* data/cleaned
   - n1_cleaned - deleted duplicates and articles before 31st October 2024 (around 34673 articles)
   - rts_latin - cleaned articles from RTS with data in Serbian latin script instead of Serbian cyrilics
* data/test
   - random_headlines.csv - 570 randomly sampled headlines from n1 dataset that I manually labeled as related and undrelated to the protests for validation
*data/related_unrelated
   - gpt_labeled_headlines_related_unrelated.csv file that includes the result of gpt API labeling
*event
   - events_extracted_n1.csv file containing events extracted from N1 headlines
   - events_extracted_rts.csv file containing events extracted from N1 headlines
   - events_extracted_manually_labeled.csv file containing events extracted from headlines and my manual check to see if the event extraction was accurate
   - events_extracted_sample_test.csv file containing a sample of events extracted from N1 headlines I used for manually testing
3. Code - contains code used for the analysis
   - News_Data_Scraping.ipynb - includes the code used for web scraping both websites
   - Data_Cleaning.ipynb - includes the code used for cleaning the datasets
   - Tokenization.ipynb - Inlcudes tokenization, lemmatization, and visualization of word count
   - Scraping_News_Articles_Full_Text.ipynb - Includes the code for scraping full texts of articles
   - GPT_API_labeling.ipynb - Code that uses GPT API for labeling headlines as related and unrelated to the protests
   - Event_Extraction.ipynb - Code that uses GPT API for event extraction
4. Test - contains code used for trying out different functions


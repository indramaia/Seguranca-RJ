
# Web Scraping News Articles from the Rio de Janeiro Security Institute to build a Word Cloud through as a NLP experiment


### Technologies
Python version 3.9
### Tools
Jupyter 
Tableau
### Services
Github

## Python Libraries
gensim
pyLDAvis
sklearn
nltk
stop_words
os
time
matplotlib
random
wordcloud
re
numpy
logging
texthero
pandas
IPython
warnings
csv
operator
warnings
tqdm
requests
BeautifulSoup
selenium
time
requests
spacy
pt_core_news_lg
collections
json

# WorkFlow
The Public Security Institute (ISP), created by Law nº 3.329, of December 28, 1999, is an autarchy directly linked to the State Secretariat for Planning and Management. With 21 years of existence, the ISP has a wealth of knowledge accumulated in the development of methodologies for analyzing data relating to Public Safety. Its mission is to produce information and disseminate research and analysis with a view to influencing and subsidizing the implementation of public security policies and ensuring social participation in the construction of these policies.

I extracted all articles published at their website.

First I used Selenium so we could open the full list of articles from the dynamic website. Then we extracted all the links and put it on a Pandas DataFrame.
Then, I used BeautifulSoup to isolate each variable for each news. After isolating and extracting news-id, date, author, title and text. I put it all in the same DataFrame.
Further, I preprocessed all the text removing stopwords, weblinks, punctuation, diacritics, digits, whitespace, NaNs and applied lowercase for all of our text.
At last I applied a Topic Model template to generate tagclouds and visualizations.

I've extracted the news using BeautifulSoup and Selenium. 

At last I created a Topic Model using LDA algorithm and generated 30 topics from our full Corpus.

Those are the tagclouds from some topics:

![word_cloud_isp](https://user-images.githubusercontent.com/65928388/145307072-62f554e7-2c72-409f-a9ac-80347e979fa4.png)
![gun](https://user-images.githubusercontent.com/65928388/145307094-ae774097-9d03-4bd4-862a-0355e4bcfeba.png)

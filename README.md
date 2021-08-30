# Flask-Web-App-for-Vertical-Search-Engine-through-Crawling-and-Indexing

Flask Web App based vertical search engine is developed which searches for articles. Overall, there are four major components:
1.	Crawling
2.	Indexing
3.	Query processing
4.	UI (Web app) 

## 1. Crawling:
For web crawling and scraping data, we've used Beautifulsoup.

## 2. Indexing:
Elasticsearch is used for indexing/ storing data extracted during the web crawling task. Data is stored incrementally as one document at a time as new requests are made and ‘h3 tags’ data is collected in bs4

## 3. Query Processing:
Elasticsearch makes it very easy to search for relevant data using its search API. In order to show relevant results to users, their search words are used in the search query of elasticsearch. We used ‘multimatch’ to search for data in both titles and urls fields of ‘research_output’ index. 

## 4. UI (Web app):
For User Interface, flask framework is used. There are two main pages of the web interface named as search.html and results.html pages. 

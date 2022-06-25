# StockSentimentAnalysis
This project of Sentiment Analysis on Financial News classifies the polarity of a given text, article or news snippet about the financial markets using VADER sentiment analysis. 
![Final Output](https://drive.google.com/uc?export=view&id=15aBMVSkrBIZfk1dU28hFuaiYlZjVNOYv)

# Working 
![Flowchart](https://drive.google.com/uc?export=view&id=1oygJPP-cJkCeqdQCVPqG4QRHAtC7gihA)

* We use the name of the company to find articles related to these companies from two websites; livemint.com and businesstimes.com. The company name is put in the search parameters and then we get all the links to the articles from both the websites regarding the company. Once we have the links, we can individually feed the content of all the articles to the sentiment analyser.
* Vader (Valence Aware Dictionary and sEntiment Reasoner) is a lexicon and rule-based sentiment analysis tool that is majorly used for understanding sentiments expressed in social media. It uses a lexicon which is a list of words that have been labelled with their corresponding semantic orientation as either positive or negative.
* Once we have the lexicon made, we feed the content of the news articles to Vader. This returns us with the sentiment score of the entire article. We can then plot this and visualize the relative sentiment of different articles and understand the relationship between the news and the sentiment that Vader calculates. 
![VADER Output](https://drive.google.com/uc?export=view&id=1jgoJdXpOBU4nr2t6siPft8Bu9hPJ8jO3)

Apart from doing sentiment analysis the notebook also shows some charts related to the selected company using the yfinance API. Based on that data we create the indicators of RSI, Bollinger Bands and MACD (Moving Average Convergence Divergence) and display it on graphs for the user to view. 
![Technical Output](https://drive.google.com/uc?export=view&id=1j0997G5rdDgbXfypuTK-IUtKgg9fkYA5)

**Note: It is possible that the webscraping does not work anymore and could throw errors if the websites were updated in some way.**

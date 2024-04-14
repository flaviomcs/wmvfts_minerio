# wmvfts_minerio
Codes of experiments carried out to predict iron ore prices through a hybrid predictive system, which uses an index obtained from the aggregation of sentiments extracted from tweets related to iron ore, based on hesitant fuzzy sets, and the number of tweets as exogenous variables for a multivariate Weighted Multivariate Fuzzy Time Series (WMVFTS) model.

The logical sequence for using the codes is:
1- “Extraindo Tweets com Python.ipynb” extracts the tweets of interest through the Twitter API.
2- “Sentiment classification with BERT and Embedding.ipynb” pre-processes the extracted tweets and obtains, through BERT sentiment analysis, the sentiment of each of them.
3- “agg_sentment.ipynb” performs the daily and monthly aggregation of sentiments obtained from tweets.
4- "Experimentos_minerio_sent.ipynb" forecasts iron ore prices through WMVFTS using as input variables only the monthly historical series of ore prices and the aggregate sentiments of tweets.
5- “Experimentos_minerio_count.ipynb” forecasts iron ore prices through WMVFTS using as input variables only the monthly historical series of ore prices and the number of tweets posted each month.
6- "Experimentos_minerio_multi.ipynb" forecasts iron ore prices through WMVFTS using as input variables the monthly historical series of ore prices, the aggregate sentiments of tweets and the number of tweets posted in each month.
7- “Estatisticas.ipynb” contains the calculation of statistics relating to variables and forecasts.
8- "rev_graf_final.ipynb" contains the graphical construction of the results.

All files that appear in the codes as called through "drive.mount('/content/drive')" are in the "dados" folder.

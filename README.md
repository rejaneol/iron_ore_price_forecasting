# iron_ore_price_forecasting
# Forecasting Commodities Prices: Iron Ore

## Summary
In this project, a time series approach was used to model and forecast iron ore prices.

## Motivation: 
As the article from Visual Capitalist shows ([From Bust to Boom: Visualizing the Rise in Commodity Prices](https://elements.visualcapitalist.com/visualizing-the-rise-in-commodity-prices/)), commodities are "the stuff that makes everything". They are important materials because all objects around us are made of one or more of them. Their prices affect how business are made and affect our daily lives through the things we need to buy.  
Steel is one of the common materials and it is made of iron ore.  
It is important to understand and try to to forecast the iron ore prices for both market and long-run capital investments planning purposes.

#### The main findings are summarized in a blog post you can read [here](https://medium.com/@reol/iron-ore-prices-forecasting-a-time-series-approach-with-pmdarima-python-package-44bcdebb5951)

## The project

The project was developed in a Python Jupyter Notebook: [iron-ore-prices-forecasting.ipynb](https://github.com/rejaneol/iron_ore_price_forecasting/blob/main/iron-ore-prices-forecasting.ipynb)  

The **packages** and versions are listed below:   
matplotlib==2.2.2  
numpy==1.19.2  
pandas==1.1.5  
pmdarima==1.8.2  
scikit-learn==0.24.2  
scipy==1.5.2  
seaborn==0.9.0  
statsmodels==0.12.2  

The project followed the structure below:  
- Exploratory Data Analysis
- Modeling  
  - Simple Modeling  
  - Modeling - tuning hyperparameters  
  - Cross-validation Modeling  
  - Final Model   
- Persisting the final model

In the _Exploratory Data Analysis_ phase, we investigated:  
1. The aspects of Iron Ore Prices historical data, both with autocorrelation and lag plots and stationarity statistical tests.    
2. Additional variables that could influence the iron ore prices (exogenous variables), like scrap prices, steel prices and China GDP, were also tested for Granger Causality.  

In the _Modeling_ phase, the pmdarima python package and its functions auto arima and cross-validation functions are used.  
An ARIMAX model was fitted and a MAPE of about 21% was found.  


## Acknowledgments
https://otexts.com/fpp2/  
https://machinelearningmastery.com/arima-for-time-series-forecasting-with-python/  
https://www.nbshare.io/notebook/136553745/Time-Series-Analysis-Using-ARIMA-From-StatsModels/  
https://www.machinelearningplus.com/time-series/arima-model-time-series-forecasting-python/  
https://github.com/alkaline-ml/pmdarima  
https://alkaline-ml.com/pmdarima/index.html  
https://medium.com/keita-starts-data-science/time-series-split-with-scikit-learn-74f5be38489e  
https://stackoverflow.com/questions/46732748/how-do-i-use-a-timeseriessplit-with-a-gridsearchcv-object-to-tune-a-model-in-sci  
https://towardsdatascience.com/time-based-cross-validation-d259b13d42b8  
https://www.analyticsvidhya.com/blog/2021/08/granger-causality-in-time-series-explained-using-chicken-and-egg-problem  
https://stats.stackexchange.com/questions/476536/interpreting-statsmodel-granger-causality-test-results-ssr-chi2test  
https://www.mathworks.com/help/econ/rolling-window-estimation-of-state-space-models.html  
https://towardsdatascience.com/an-end-to-end-project-on-time-series-analysis-and-forecasting-with-python-4835e6bf050b   
https://machinelearningmastery.com/make-sample-forecasts-arima-python/  
https://www.oecd.org/industry/ind/steel-market-developments-Q4-2020.pdf



# Singapore Covid-19 Prediction
**Done by Prannaya Gupta**

In this project, we analyze the Singapore Covid-19 data using multiple Time Series Models. The prediction analyses data from online and runs different models to find an optimum prediction for the Covid-19 Slope. We predicted the COVID-19 outbreak trajectory for Singapore in the next 6 months (from September 2020 this is very outdated). We retrieved data from OWID and used ARIMA, a modified version of Double Exponential Smoothing and the Prophet API to test and evaluate the data, and made predictions. This project was done as part of the Singapore Problem X (PX) Challenge. You can look into it [here](PX.ipynb). 

## Workspace

### Imports and Data Preparation

As the name suggests, this section deals with importing important libraries, retrieving the data from the [OWID Github .csv file](https://raw.githubusercontent.com/owid/covid-19-data/master/public/data/owid-covid-data.csv). Here, we also account for the time lag in the recording of data by OWID.

### Testing of Data

Here, we test the data in order to find out many different possible curves to use for the prediction. Click [here](https://towardsdatascience.com/the-complete-guide-to-time-series-analysis-and-forecasting-70d476bfe775) for info regarding why this series of tests is conducted and what the significance is.

### ARIMA Prediction

We use the ARIMA method to predict the best possible with the least MAPE score. Once again, click [here](https://towardsdatascience.com/the-complete-guide-to-time-series-analysis-and-forecasting-70d476bfe775) for info regarding the significance of this test.

### Double Exponential Smoothing

This is a modified algorithm for Time Series Analysis. This algorithm was made by me and does not follow any normal method. I use my data from the double exponential smoothing test and used the very accurate curve to predict to a further extent. My algorithm uses trends and levels from the previous 10 days.

### Prophet Prediction

I use Facebook's Prophet API to generate a model. This was mainly inspired by info from [here](https://www.digitalocean.com/community/tutorials/a-guide-to-time-series-forecasting-with-prophet-in-python-3).

### Evaluation of Data

Here, I used all previous data to average out and make an overally data prediction. The cases individually until October 1st are all laid out and there is also an accompanying graph.



## Some Suggestions
Open the document **in colab** since there are a lot of unnecessary datasets that cannot be minimised in Github. 

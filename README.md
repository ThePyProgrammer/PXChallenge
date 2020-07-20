# PXChallenge
This repository is mainly predictions of Covid-19 in Singapore for the PX Challenge

You can look into it [here](PX.ipynb).

## Table Of Contents:
| Section| Description|
| ------------- |:-------------:|
|Imports and Preparation of data|As the name suggests, this section deals with importing important libraries, retrieving the data from the [OWID Github .csv file](https://raw.githubusercontent.com/owid/covid-19-data/master/public/data/owid-covid-data.csv). Here, we also account for the time lag in the recording of data by OWID.|
|Testing of data|Here, we test the data in order to find out many different possible curves to use for the prediction. Click [here](https://towardsdatascience.com/the-complete-guide-to-time-series-analysis-and-forecasting-70d476bfe775) for info regarding why this series of tests is conducted and what the significance is.|
|ARIMA Prediction|We use the ARIMA method to predict the best possible with the least MAPE score. Once again, click [here](https://towardsdatascience.com/the-complete-guide-to-time-series-analysis-and-forecasting-70d476bfe775) for info regarding the significance of this test.|
|Double Exponential Smoothing (modified) Prediction|This algorithm was made by me and does not follow any normal method. I use my data from the double exponential smoothing test and used the very accurate curve to predict to a further extent. My algorithm uses trends and levels from the previous 10 days.|
|Predicting using Prophet|I use Facebook's Prophet to generate a model. This was mainly inspired by info from [here](https://www.digitalocean.com/community/tutorials/a-guide-to-time-series-forecasting-with-prophet-in-python-3).|
|Evaluation of Data|Here, I used all previous data to average out and make an overally data prediction. The cases individually until October 1st are all laid out and there is also an accompanying graph.|

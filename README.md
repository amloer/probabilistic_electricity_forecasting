# Probabilistic short-term electric load forecasting with pinball loss guided machine learning models

Electricity supply and demand should be balanced at any time. Imbalances can lead to additional costs for electricity suppliers. Ongoing developments in electricity markets, caused by the energy transition, increase volatility in electricity demand. In this context, the research questions arise, whether uncertainty in short-term electrical load forecasts can be quantified and which variables are the most relevant when predicting uncertainty in electricity forecasts. 

To answer these research questions, real-world electricity consumption records were obtained from the German transmission system operator Amprion GmbH, Dortmund, Germany and weather data was obtained from the weather service Deutscher Wetterdienst, Offenbach, Germany. The datasets covered the time frame from the 1st of January 2018 till the 31st of March 2019.

The quantile loss guided probabilistic forecasting approach was used to include uncertainty into forecasts. The three models ARIMA with confidence intervals, quantile gradient boosting and quantile LSTM were created to predict quarter-hourly electricity consumption up to 24 hours ahead. The quantile forecasts were compared based on their average pinball loss score.

Among the three models, the pinball loss-guided LSTM performed the best in computing quantile predictions. Furthermore, data on historical consumption and temperature are relevant when making short-term probabilistic load forecasts.
The proposed models can be used by managers of electricity supplying companies to manage operational risk. Specific areas of application could be demand side management or electricity purchasing.

**Data sources:**
- consumption: https://www.amprion.net/Grid-Data/Demand-in-Control-Area/ (accessed 01.06.2021)
- weather: https://www.dwd.de/DE/leistungen/klimadatendeutschland/klarchivtagmonat.html;jsessionid=2A0D0FC8D5BCAE83E9879C48F9A6972E.live21063?nn=16102 (accessed 01.06.2021)

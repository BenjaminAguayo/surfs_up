# Challenge 9: Surf's up

## 1. Overview of statistical analysis 
The purpose of this analysis is to gather information about temperature trends before opening the surf shop to determine if the surf and ice cream shop business is sustainable year-round.


## 2. Results
##### A) The results of June
![June_Temps](https://user-images.githubusercontent.com/102047412/173207858-e3643e19-0d01-429e-8e78-8d5ed7c6074c.png)

##### B) The results of December
![Dec_Temps](https://user-images.githubusercontent.com/102047412/173207861-5d6fe0d0-7ab4-48ea-a048-de017bb8232a.png)

- Mean temperature in June was 23.8ºC whereas in December was 21.6ºC, so there are less than 3ºC of difference on average.
- Maximum temperature in June was 29.4ºC, the hotest measurment, and maximum temperature in December was 28.3ºC.
- Minimum temperature in June was 17.7ºC, the hotest measurment, and maximum temperature in December was 13.3ºC.

## 3. Summary
According to the obtained results, the temperature seems suitable for opening the surf shop, since the weather is trending warm, there are no temeratures below 13ºC, and it is rather hoter.

In order to gather more weather data for june and december the following queries can be used to determine the precipitations and elaborate the outcome of investigation.
```python
precipitation_jun = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==6).all()
precipitation_dec = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==12).all()
```

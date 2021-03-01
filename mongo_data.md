# Mongodata API reference :snowflake:


![Image of Telosair](https://github.com/Potsdam-Sensors/Telosair/blob/main/img/telosair.png)



###  Import Mongodata :smiley_cat:

```python
 from mongodata import mongodata
```

###  Import Authentication for database :smiley_cat:

```python
 mongodata=mongodata.TAAPI(host='peyton.potsdamsensors.com',   collection_name='ualbany',username='XXX',password='XXX')
```

###  Query data from certain time and certain devices :smiley_cat:
* Type your devices id first, exp: 777,771, etc
* Type your time range

```python
 data=mongodata.concat(777,771,772,
                       startTime='2021-02-18 11:22:00',
                       endTime='2021-03-01 13:00:00')
```

###  Show the Timeseries plot of your data :smiley_cat:
* data is your data 
* then type the channels you need to plot , exp: tvoc, temp etc.

```python
 mongodata.plot_timeSeries(data,'mpn03um')
```


### Save your data to csv  :smiley_cat:
* data will saved in your working path

```python
data.to_csv('data.CSV')
```
# Mongodata API reference :snowflake:


![Image of Telosair](https://github.com/Potsdam-Sensors/Telosair/blob/main/img/telosair.png)



### :smiley_cat:  Import Mongodata 

```python
 from mongodata import mongodata
```

### :smiley_cat: Import Authentication for database 
* fill in your collection name (Remove XXX)
* fill in your username  (Remove XXX)
* fill in your password  (Remove XXX)

```python
 mongodata=mongodata.TAAPI(host='peyton.potsdamsensors.com',   collection_name='xxx',username='XXX',password='XXX')
```

### :smiley_cat: Query data from certain time and certain devices 
* Type your devices id first, exp: 777,771, etc
* Type your time range

```python
 data=mongodata.concat(777,771,772,
                       startTime='2021-02-18 11:22:00',
                       endTime='2021-03-01 13:00:00')
```

### :smiley_cat: Save your data to csv  
* data will saved in your working path

```python
data.to_csv('data.CSV')
```

### :smiley_cat: Show the Timeseries plot of your data 
* data is your data 
* then type the channels you need to plot , exp: tvoc, temp etc.

```python
 mongodata.plot_timeSeries(data,'mpn03um')
```


### :smiley_cat: Show the HTML Timeseries plot of your data 
* data is your data 
* then type the channels you need to plot , exp: tvoc, temp etc.

```python
 mongodata.plot_timeSeriesHtml(data,'mpn03um')
```
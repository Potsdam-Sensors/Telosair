# Mongodata API reference :snowflake:


![Image of Telosair](https://github.com/Potsdam-Sensors/Telosair/blob/main/img/telosair.png)



###  Import Mongodata :smiley_cat:

```python
 from mongodata import mongodata
```

###  Import Authentication for database :smiley_cat:

```python
 mongodata=mongodata.TAAPI(username='XXX',password='XXX')
```

###  Query data from certain time and certain devices :smiley_cat:

```python
 data=mongodata.concat(777,771,772,
                       startTime='2021-02-18 11:22:00',
                       endTime='2021-03-01 13:00:00')
```
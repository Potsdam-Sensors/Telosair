

| Header | Description | Unit | Notes |
| --- | --- | --- | --- |
| `_id` | Database ID (Ignore) | | |
| `deviceType` | 2 represent Duet (we have other types for other measurement units)|| |
| `device_id` | Serial ID of sensor (this is information required for data access from that unit)|| |
| `unix` | Timestamp by the gateway|seconds since Jan 01 1970. | |
| `gateway_serial` | Serial ID of gateway|| |
| `pm10_t` | PM 1.0 from "top PM sensor"  (There are two PM sensors - labeled "top" and "bottom")|ug/m^3| |
| `pm25_t` | PM2.5 from "top PM sensor"|ug/m^3| |
| `pm100_t` | PM10 from "top PM sensor"|ug/m^3| |
| `pn03_t` | Number concentration of particles larger than 0.3 um for "top sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn05_t` | Number concentration of particles larger than 0.5 um for "top sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn10_t` | Number concentration of particles larger than 1.0 um for "top sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn25_t` | Number concentration of particles larger than 2.5 um for "top sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn50_t` | Number concentration of particles larger than 5.0 um for "top sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn100_t` | Number concentration of particles larger than 10.0 um for "top sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pm10_b` | PM 1.0 from "bottom PM sensor"  (There are two PM sensors - labeled "bottom" and "bottom")|ug/m^3| |
| `pm25_b` | PM2.5 from "bottom PM sensor"|ug/m^3| |
| `pm100_b` | PM10 from "bottom PM sensor"|ug/m^3| |
| `pn03_b` | Number concentration of particles larger than 0.3 um for "bottom sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn05_b` | Number concentration of particles larger than 0.5 um for "bottom sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn10_b` | Number concentration of particles larger than 1.0 um for "bottom sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn25_b` | Number concentration of particles larger than 2.5 um for "bottom sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn50_b` | Number concentration of particles larger than 5.0 um for "bottom sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `pn100_b` | Number concentration of particles larger than 10.0 um for "bottom sensor"|#/0.1 L|Divide by 100 to get #/cc |
| `temp` | Temperature|C or F| |
| `hum` | Humidity|%| |
|`pressure`| Pressure in of water | | |
|`tvoc`| Total VOCs|ppb| |	
|`eco2`| equivalent CO2	| ppm| |	
|`rawh2`||||			
|`rawethanol`|	Currently provide absolute CO2 - use this channel for more accurate CO2 value |	ppm||	
|`lastRssi`| Radio signal strength|	dB|	Good signal: 0 to -100|
|`lastSNR`|	Signal noise ratio ||typical ~ 5|
|`hops`|	Number of nodes needed to reach gateway		 (0 is direct connection; 1 - one intermediate link, etc)|||
|`mpn03um`|	merged value of PN03 |	#/0.1 L |	when the two values (pn03_t and pn03_b) are within 15% of each other|
|`mpm25`|	merged value of pm2.5 |ug/m^3|	when the two values (pm25_t and pm25_b) are within 15% of each other|
|`time_gap`|	Gap in time between two measurements |seconds|large time gaps could mean poor connectivity; ideally less than 10 seconds|
|`time_dif`| compare in the current time value with privious time value	seconds|||	
|`temp_dif`|	compare in the current temperature value with privious temperature value |c||	
|`hum_dif`|	compare in the current humidity value with privious humidity value|	%||	
|`pressure_dif`|	compare in the current pressure value with privious pressure value ||		
|`tvoc_dif`| compare in the current TVOC value with privious TVOC value| ppb||	
|`mpn03um_dif`|	compare in the current particle number concentration value with privious particle number concentratio  value|||		
|`Date`|	Date|||		
|`month`|	Month|||		
|`weekday`|	Weekday	|||	
|`day_of_week`|	day of week|||		
|`hour`|	hours	|||	
|`days`|	days|||		
|`pt_status`|	plantower health status|||		
|`pt_level`|	plantower health status|||		
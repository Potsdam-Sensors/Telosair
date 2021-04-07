

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
# Historical Weather Query

Quick and dirty module to query Weather Canada's website for historical daily highs and precipitation. There are probably better solutions to this out there that query a proper API.

## Usage:
```from vanweather import get_weather_range
wdf = get_weather_range((2017,4),(2017,6))
```

```get_weather_range``` takes two (year,month) tuples and returns and pandas dataframe with columns: 

```['Max Temp', 'Min Temp', 'Mean Temp', 'Heat Deg Days', 'Cool Deg Days', 'Total Rainmm', 'Total Snowcm', 'Total Precipmm', 'Snow on Grndcm', 'Dir of Max Gust10's deg', 'Spd of Max Gustkm/h']```
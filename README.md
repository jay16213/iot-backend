# 2017 IOT Weather underground backend
## Data field
### A field with prefix 'fore_' means that it is a forecast infomation
- location: string
- condition: string
- temp_c: float
- relative_humidity: string
- icon_url: string
- fore_condition: string
- fore_temp: string

## Method
- init: give a location and it will pull the current weather condition from api
- update: update the current weather condition
- getForecast(hour: int): get the forecast info from api, should give parameter 'hour' to get the forecast at 'hour' o'clock

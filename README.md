# 2017 IOT Weather underground backend

## Class Weather
### Import
- `from weather import Weather`

### Constructor
- `varName = Weather(location_str)`
- the constructor will call getCurrentConditions()

### Data field
- current condition
    - location: string
    - condition: string
    - temp_c: float
    - humidity: string
    - wind_kph: float
    - icon: string
    - icon_url: string

- after calling getHourForecast, you will have the following data
    - hour_condition: string
    - hour_temp: string
    - hour_humidity: string
    - icon: string
    - hour_icon_url: string

- after calling getWeekForecast, you will have the following data
    - fore_week: list of directory
        - temp_high: float
        - temp_low: float
        - conditions: string
        - icon: string
        - icon_url: string
    - use fore_week[index][key] to get value. e.x fore_week[0]['temp_high']

### Method
- getCurrentConditions(): update the current weather condition

- getHourForecast(hour: int): get the forecast info from api, should give parameter 'hour' to get the forecast at 'hour' o'clock

- getWeekForecast(): get 10 days forecast info

## Class Distance
### Import
- `from distance import Distance`

### Constructor
- `varName = Distance(origin, destination)`

### Data field
- distance: string
- duration: string


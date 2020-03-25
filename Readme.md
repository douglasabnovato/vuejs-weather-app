Weather App
- Aplicativo do Tempo
- Api [Open Weather Map](https://openweathermap.org/)
https://openweathermap.org/current <br/>
By geographic coordinates<br/>
- API call:<br/>
api.openweathermap.org/data/2.5/weather?lat={lat}&lon={lon}&appid={your api key}
- Parameters:<br/>
lat, lon coordinates of the location of your interest
- Examples of API calls:<br/>
api.openweathermap.org/data/2.5/weather?lat=35&lon=139
- API response:
````javascript
{"coord": { "lon": 139,"lat": 35},
  "weather": [
    {
      "id": 800,
      "main": "Clear",
      "description": "clear sky",
      "icon": "01n"
    }
  ],
  "base": "stations",
  "main": {
    "temp": 281.52,
    "feels_like": 278.99,
    "temp_min": 280.15,
    "temp_max": 283.71,
    "pressure": 1016,
    "humidity": 93
  },
  "wind": {
    "speed": 0.47,
    "deg": 107.538
  },
  "clouds": {
    "all": 2
  },
  "dt": 1560350192,
  "sys": {
    "type": 3,
    "id": 2019346,
    "message": 0.0065,
    "country": "JP",
    "sunrise": 1560281377,
    "sunset": 1560333478
  },
  "timezone": 32400,
  "id": 1851632,
  "name": "Shuzenji",
  "cod": 200
}
````

:. de Igor Halfeld em [Canal dotNET](https://www.youtube.com/watch?v=C_6vfcGcHHI)

>@douglasabnovato
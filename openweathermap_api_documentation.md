# API Documentation – OpenWeatherMap – Current Weather by City Name

## OVERVIEW:
This returns the current weather data for a specific city. The temperature, humidity, weather condition is also added. In this example we retrieve weather data for Chennai. GET request is used to retrieve the data in JSON format. The tool that is used here is the POSTMAN. 
## API : 
Open Weather Map
## HTTP Method:
GET
## BASE URL:
`https://api.openweathermap.org`
## END POINT:
/data/2.5/weather
## PARAMETERS AND THEIR VALUES:
q=chennai&appid={api_key}&units=metric
-	q, is the parameter used and it stores the city name. City name we have used here is, Chennai. 
-	appid, is the parameter used and it stores the api authorization key. The API key from OpenWeatherMap.
-	units, is the parameter used and it stores the unit of measurement. Metric gives the temperature in, Celsius and the windspeed in meter/sec. 
POSTMAN Setup:
-	GET method is used. 
-	Select auth type as API Key. 
-	Select Query Params from the dropdown
-	Type the key and value in the respective boxes. 
-	Other params, q:Chennai, units:metric

## FULL HTTP REQUEST EXAMPLE:
**GET** https://api.openweathermap.org/data/2.5/weather?q=chennai&appid={}&units=metric
## RESPONSE:
We get response in JSON format.
```

"coord": {
        "lon": 80.2785,
        "lat": 13.0878
    },
    "weather": [
        {
            "id": 804,
            "main": "Clouds",
            "description": "overcast clouds",
            "icon": "04d"
        }
    ],
    "base": "stations",
    "main": {
        "temp": 31.48,
        "feels_like": 38.48,
        "temp_min": 31.48,
        "temp_max": 31.48,
        "pressure": 1002,
        "humidity": 69,
        "sea_level": 1002,
        "grnd_level": 1000
    },
    "visibility": 10000,
    "wind": {
        "speed": 4.41,
        "deg": 245,
        "gust": 5.49
    },
    "clouds": {
        "all": 100
    },
    "dt": 1753091766,
    "sys": {
        "country": "IN",
        "sunrise": 1753057291,
        "sunset": 1753103321
    },
    "timezone": 19800,
    "id": 1264527,
    "name": "Chennai",
    "cod": 200
}
```
## NOTES:
This API retrieves real time weather information for any specific city. So, correct parameters and valid authorization key is required for successful response. 


## STATUS CODE AND MESSAGE:
200	 OK

## ERROR RESPONSES:
We may get error responses like 401 Unauthorized, 404 Not Found, 400 Bad Request in case of using wrong authorization key, wrong city mentioned or if the parameters are missing and invalid.  

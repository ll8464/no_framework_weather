# Overview

The goal of this site is to create an easy to read landing page that simply tells the weather.

Technologies include: HTML, CSS, JavaScript, and Bootstrap.

APIs Used:
Unsplashed - for random background images.
source.unsplash.com
In the style.css file, the background url is: https://source.unsplash.com/1600x900/?nature,water

OpenWeatherMap.org - the Weather API
Example of call using city name:
http://api.openweathermap.org/data/2.5/weather?q=houston&units=imperial&appid=7a3d4408ad3936a73e4a95fd6bd93bd1

## API Explanation

The flow of a call goes as follows: a search querySelector is activated, via click or Enter, and calls the weather.search() method.

weather.search() calls fetchWeather by passing through the value that was inputed into the search bar as a parameter.

weather.fetchWeather then fetches data from the openWeatherMap API, then converts it into json data, and finally passes that json data to the weather.displayWeather() method as a parameter.

Finally, displayWeather() updates all html content via querySelectors based on the json data received from openWeatherMap. Also, this is where the background images from unsplash receive appropriate location data and then are updated.

## Future

The API is in a good place as it stands. It was an excellent venture into API calls, javaScript, and HTML/CSS.

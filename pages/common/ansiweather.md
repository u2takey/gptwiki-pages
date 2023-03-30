# ansiweather 
## chatgpt 
The command "ansiweather" is a command-line utility tool that provides weather information in the terminal. It is an open-source tool that uses the API of OpenWeatherMap to fetch weather data and display it in a formatted manner.

When you run the "ansiweather" command in your terminal, it will display information about the current weather conditions of your location or any other location specified. It will show the current temperature, wind speed, humidity, and conditions like sunny, cloudy, rainy, etc.

Additionally, ansiweather provides a forecast of the weather for the next few hours, upcoming days, and a summary of the day, i.e., sunrise and sunset times, max and min temperature, etc.

Moreover, ansiweather can be customized in many ways. For instance, users can change the colors used for various parts of the output, choose the unit of temperature, set the refresh rate for automatic updates, and much more.

Overall, the ansiweather command gives terminal users quick and easy access to weather information without having to open another app or website, making it a useful tool for those who want to stay updated on the weather conditions. 

## tldr 
 
> A shell script for displaying the current weather conditions in your terminal.
> More information: <https://github.com/fcambus/ansiweather>.

- Display a forecast using metric units for the next five days for Rzeszow, Poland:

`ansiweather -u {{metric}} -f {{5}} -l {{Rzeszow,PL}}`

- Display a forecast showing symbols and daylight data for your current location:

`ansiweather -s {{true}} -d {{true}}`

- Display a forecast showing wind and humidity data for your current location:

`ansiweather -w {{true}} -h {{true}}`

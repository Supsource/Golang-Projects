# Weather Tracker API with Go
This project is a simple API that retrieves the current weather data for a given location. The API is built using Go and integrates with the OpenWeatherMap API to retrieve the weather data.
## Getting Started
To run the API, you'll need to have Go installed on your machine. You'll also need to sign up for an OpenWeatherMap API key, which you can do for free on the [OpenWeatherMap](https://openweathermap.org/api) website.
Once you have Go and an OpenWeatherMap API key set up, follow these steps to run the API:
1. Clone the repository to your local machine.
2. Create a file named `.apiConfig`in the root directory of the project.
3. Add your OpenWeatherMap API key to the `.apiConfig` file in the following format:
```json
{
  "OpenWeatherMapApiKey": "your-api-key-here"
}
```
4. In your terminal, navigate to the project directory and run the following command to start the API:
```go
go run main.go
```
5. The API will start running on `http://localhost:8082`.
## Using the API
To retrieve the current weather data for a location, send a GET request to the `/weather` endpoint with the name of the city in the URL path. For example, to retrieve the weather data for New York City, send a GET request to `http://localhost:8080/weather/newyork`.
<br><br>
The API will return a JSON response with the following structure:
```json
{
  "name": "New York",
  "main": {
    "temp": 283.15
  }
}
```
The name field contains the `name` of the city, and the `temp` field contains the current temperature in Kelvin.

## Contributing
If you'd like to contribute to the project, please feel free to submit a pull request. Before submitting a pull request, please make sure your changes are thoroughly tested and meet the project's code standards.







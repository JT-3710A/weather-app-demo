# Weather App Demo

## Project Description

This is a simple, responsive web application that displays current weather conditions and forecasts for any city worldwide. It leverages the OpenWeather API to fetch real-time weather data and provides a clean, intuitive user interface.

## Features

-   **City Search**: Search for weather information by city name.
-   **Geolocation**: Automatically detect and display weather for your current location.
-   **Current Weather**: Shows temperature, humidity, wind speed, and weather description.
-   **Hourly Forecast**: Displays hourly temperature and conditions (limited by OpenWeather's free tier).
-   **Daily Forecast**: Provides a multi-day forecast (limited by OpenWeather's free tier).
-   **Recent Searches**: Keeps a history of recently searched cities for quick access.
-   **Responsive Design**: Adapts to different screen sizes (desktop, tablet, mobile).
-   **Loading & Error Handling**: Provides visual feedback during data fetching and displays error messages for invalid inputs or API issues.
-   **Interactive Charts**: Visualizes hourly temperature, humidity, and AQI using Chart.js.

## Technologies Used

-   **HTML5**: For structuring the web content.
-   **CSS3 (Tailwind CSS)**: For styling and responsive design.
-   **JavaScript (Vanilla JS)**: For dynamic functionality and API interactions.
-   **OpenWeather API**: For fetching weather data.
-   **Chart.js**: For creating interactive weather charts.

## Setup and Installation

To run this project locally, follow these steps:

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
    ```
    (Replace `YOUR_USERNAME` and `YOUR_REPO_NAME` with your actual GitHub username and repository name)

2.  **Navigate to the project directory**:
    ```bash
    cd "weather-app-demo"
    ```

3.  **Obtain an OpenWeather API Key**:
    -   Go to the [OpenWeather website](https://openweathermap.org/api).
    -   Sign up for a free account.
    -   Generate an API key. (Note: It might take a few minutes for the API key to become active).

4.  **Configure your API Key**:
    -   Open the `index.html` file in a text editor.
    -   Locate the JavaScript section (around line 81) where `API_KEY` is defined.
    -   Replace `"YOUR_OPENWEATHER_API_KEY"` with your actual API key:

    ```javascript:e%3A%5Cweather%20app%20using%20open%20metro%5Cindex.html
    // ... existing code ...
    const config = {
        API_KEY: "YOUR_OPENWEATHER_API_KEY", // Replace with your actual API key
        BASE_URL: "https://api.openweathermap.org/data/2.5/",
        GEO_URL: "https://api.openweathermap.org/geo/1.0/",
    };
    // ... existing code ...
    ```

5.  **Open the application**:
    -   You can simply open the `index.html` file directly in your web browser.
    -   Alternatively, for a local server environment (recommended for development):
        ```bash
        python -m http.server 8000
        ```
        Then, open your browser and go to `http://localhost:8000`.

## Usage

-   Enter a city name in the search bar and press Enter or click the search button.
-   Click the "Use My Location" button to get weather data based on your current geographical position.
-   Navigate between "Current", "Hourly", and "Daily" views to see different forecast details.
-   Recently searched cities will appear below the search bar for quick access.

## API Limitations

-   The free tier of the OpenWeather API has limitations on the number of calls and the granularity of forecast data. You might only get 4-5 days of daily forecast and 3-hour step hourly forecast data.

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests.

## License

This project is open-source and available under the [MIT License](LICENSE). (You might want to add a LICENSE file if you haven't already).

## Acknowledgments

-   [OpenWeather](https://openweathermap.org/) for providing the weather API.
-   [Tailwind CSS](https://tailwindcss.com/) for simplifying styling.
-   [Chart.js](https://www.chartjs.org/) for data visualization.
# Real-Time Weather Monitoring System

## Project Overview
This project is a real-time data processing system that monitors weather conditions in major Indian cities using the OpenWeatherMap API. It retrieves weather data at configurable intervals, processes the data to provide daily rollups and aggregates, and raises alerts based on user-defined thresholds.

The system is developed using Python and includes visualizations and a simple alerting mechanism to summarize weather trends and notify users of significant conditions.

## Features
- **Weather Data Retrieval**: Fetches real-time weather data for cities like Delhi, Mumbai, Chennai, Bangalore, Kolkata, and Hyderabad.
- **Data Processing**: Converts temperature values from Kelvin to Celsius and extracts relevant weather parameters.
- **Daily Rollups and Aggregates**: Calculates average, maximum, and minimum temperatures and identifies the dominant weather condition for each day.
- **Alerting System**: Allows users to define thresholds for weather conditions (e.g., temperature) and raises alerts when thresholds are breached.
- **Visualization**: Displays daily summaries, historical trends, and alerts using visual tools.
-  ## Visualization Features
System Setup: Initializes and connects to the OpenWeatherMap API using a valid API key.
Data Retrieval: Simulates API calls at configurable intervals to retrieve and parse weather data for specified locations.
Temperature Conversion: Converts temperature values from Kelvin to Celsius or Fahrenheit based on user preference.
Daily Weather Summary: Simulates weather updates over several days and calculates average, maximum, minimum temperatures, and dominant weather conditions.
Additional Parameters: Supports retrieval and analysis of additional weather parameters such as humidity and wind speed.
5 days Weather Forecast

## Requirements
- Python 3.x
- Python Libraries:
  - `requests`: For making API requests to OpenWeatherMap.
  - `python-dotenv`: For managing environment variables.
  - `matplotlib` (optional): For visualizations.
  - `pandas` (optional): For data processing.

## Setup Instructions

### 1. Clone the Repository
```bash
```https://github.com/Deepakkumarpradhann/Application-2-Real-Time-Data-Processing-System-for-Weather-Monitoring-with-Rollups-and-Aggregates

### 2. Create and Activate a Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables
- Create a `.env` file in the project root with the following content:
  ```
  API_KEY=os.getenv(6027866698d0c4a0e2b6a0f4218ae673)
  ```
  Replace `os.getenv(6027866698d0c4a0e2b6a0f4218ae673)` with your actual OpenWeatherMap API key.

### 5. Run the Application
```bash
python3 main.py
```

## Usage
- The script fetches weather data for predefined cities every 5 minutes.
- It calculates daily summaries, such as average, maximum, and minimum temperatures, as well as the dominant weather condition.
- Alerts are printed to the console or can be extended to send email notifications.

## Example Output
```
City: Delhi, Temp: 31.05000000000001°C, Feels Like: 32.900000000000034°C, Condition: Haze
City: Mumbai, Temp: 29.99000000000001°C, Feels Like: 35.01000000000005°C, Condition: Haze
City: Chennai, Temp: 29.610000000000014°C, Feels Like: 36.610000000000014°C, Condition: Mist
City: Bangalore, Temp: 25.980000000000018°C, Feels Like: 25.980000000000018°C, Condition: Rain
City: Kolkata, Temp: 29.970000000000027°C, Feels Like: 34.97000000000003°C, Condition: Mist
City: Hyderabad, Temp: 27.230000000000018°C, Feels Like: 29.640000000000043°C, Condition: Haze

...
```
# Configurable Alerting System
- Users can set custom thresholds for weather conditions, such as:
  - Alert if the temperature exceeds 35°C for two consecutive readings.
- Continuously tracks the latest weather data and compares it with the thresholds.
- If a threshold is breached, trigger an alert for the current weather conditions.
- Alerts could be displayed on the console or sent through an email notification system (implementation details are left open-ended).


## Visualizations
- Daily weather summaries and trends can be visualized using tools like `matplotlib`.
- Example visualizations include line charts for temperature trends and bar charts for dominant weather conditi


## Testing
- **Unit Tests**: Validate temperature conversion and data processing.
- **Mocking API Responses**: Use mock data to test the application without hitting the actual OpenWeatherMap API.

<!---
Deepakkumarpradhann/Deepakkumarpradhann is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

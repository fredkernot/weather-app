# 🌦️ Weather CLI Tool

Weather CLI Tool is a Python-based command-line application for fetching and displaying real-time weather data for any city using the [OpenWeather API](/https://openweathermap.org/). It offers a clean, visually-appealing output with weather icons, emojis, and formatted text for a better user experience.

## Features
- 🌍 **Real-Time Weather**: Fetch current weather data for any city worldwide.
- 📏 **Unit Conversion**: Supports both metric (Celsius) and imperial (Fahrenheit) temperature units.
- 🎨 **Stylish CLI Output**: Displays weather icons and uses ANSI excape codes for coloured, formatted text.
- 🔑 **Secure API Key Management**: Handles API keys securely using `configparser` and `.gitignore`.

## 🧠 What I Learned

While building this tool, I gained experience with:
- Developing a **functional CLI tool** in Python.
- Using argparse for command-line argument parsing.
- Managing secrets securely with configparser and configuration files.
- Making API calls with `urllib` and handling responses in JSON format.
- Enhancing CLI visuals with emojis, ANSI escape codes, and Python’s f-strings.

## Getting Started

#### Prerequisites
Ensure you have Python 3.6 or higher installed. You can check your version with:

```bash
python3 --version
``` 
#### Clone the Repository
Clone the repository to your local machine:
```bash
git clone https://github.com/your-username/weather-cli-tool.git
cd weather-cli-tool
```
#### Set up your OpenWeather API Key
1. Create an account at [OpenWeather](/https://openweathermap.org/ )
2. Generate your free API key from the [API keys page](/https://home.openweathermap.org/api_keys)
3. Add your API key to a `secrets.ini` file in the project root:
```ini
[openweather]
api_key=<YOUR_API_KEY>
```
4. Ensure `secrets.ini` is listed in your `.gitignore` file to keep it secure.

## Usage
Run the Weather CLI Tool with the following syntax:
```bash
python3 weather.py <city> [-i | --imperial]
```

#### Examples:
```bash
python3 weather.py london
```
```bash
python3 weather.py "new york" --imperial
```

#### Sample Output
```plaintext
London  🌧️
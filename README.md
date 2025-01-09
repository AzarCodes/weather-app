# Weather App

## Features
- Fetch weather data for any city worldwide.
- Displays temperature, weather description, humidity, and wind speed.

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/weather-app.git
cd weather-app
```

### 2. Install Dependencies
Ensure you have Python installed on your system. Install the required dependencies using:
```bash
pip install -r requirements.txt
```

### 3. Run the Application Locally
Start the Flask server by running:
```bash
python app.py
```

The app will be available at:
```
http://127.0.0.1:5000
```

### 4. Test the Application
- Open the app in your browser.
- Enter a city name in the input field and click **Get Weather**.
- Weather details will be displayed.

## Deployment on Render

### Steps to Deploy

1. **Push the Code to GitHub**:
   - Initialize a Git repository if you haven’t already:
     ```bash
     git init
     git add .
     git commit -m "Initial commit"
     ```
   - Push the code to a GitHub repository:
     ```bash
     git remote add origin https://github.com/your-username/weather-app.git
     git push -u origin main
     ```

2. **Set Up Render**:
   - Log in to [Render](https://render.com/) and create a new **Web Service**.
   - Link your GitHub repository.
   - Specify the **build command**:
     ```bash
     pip install -r requirements.txt
     ```
   - Specify the **start command**:
     ```bash
     python app.py
     ```

3. **Environment Variables**:
   - Add your OpenWeatherMap API key as an environment variable:
     ```
     Name: API_KEY
     Value: your_openweathermap_api_key
     ```

4. **Deploy**:
   - Render will automatically build and deploy your application.
   - After deployment, Render will provide you with a live URL to access your app.

## License
MIT License

# 🌦️ Weather API Setup Guide

## Getting Your OpenWeatherMap API Key

### Step 1: Create Account
1. Go to [OpenWeatherMap](https://openweathermap.org/api)
2. Click "Sign Up" and create a free account
3. Verify your email address

### Step 2: Get API Key
1. Log in to your OpenWeatherMap account
2. Go to "My API Keys" section
3. Copy your default API key (or create a new one)

### Step 3: Add to Environment
1. Open `.env.local` file in your project root
2. Replace `your_openweather_api_key_here` with your actual API key:
   ```
   OPENWEATHER_API_KEY=your_actual_api_key_here
   ```

### Step 4: Restart Development Server
```bash
npm run dev
```

## Free Tier Limits
- 1,000 API calls per day
- 60 calls per minute
- Current weather data
- 5-day forecast

## Features Available
✅ **Current Weather Data**
- Temperature, humidity, pressure
- Wind speed and direction
- Weather description
- Sunrise/sunset times

✅ **5-Day Forecast**
- Daily temperature predictions
- Humidity and rainfall data
- Weather conditions

✅ **Farming Recommendations**
- Temperature-based alerts
- Humidity warnings
- Wind advisories
- Irrigation suggestions

## API Endpoints Used
- Current Weather: `/data/2.5/weather`
- 5-Day Forecast: `/data/2.5/forecast`

## Fallback System
If the API key is invalid or API is down, the system automatically falls back to simulated weather data to ensure the application continues working.

## Usage in Components
```typescript
// Use the LiveWeatherWidget component
import LiveWeatherWidget from './components/LiveWeatherWidget'

<LiveWeatherWidget city="Your City" />
```

## Troubleshooting
- **Invalid API Key**: Check if the key is correctly added to `.env.local`
- **Rate Limit**: Free tier has 60 calls/minute limit
- **City Not Found**: Try using different city name formats
- **No Data**: Check browser console for error messages

---
🚜 **FarmTech Pro - Smart Agriculture with Live Weather Data!** 🌱
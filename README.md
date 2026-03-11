# 🌦️ Weather Dashboard (React + Vite + TailwindCSS)

A real-time weather dashboard built using **React**, **Vite**, and **Tailwind CSS**.  
This app displays live weather information for 275+ predefined popular locations worldwide. Users can search, save favorites, and enjoy a visually adaptive interface based on the weather conditions.

---

## 🧩 Overview

The app fetches real-time weather data using a custom React hook and displays:

- Current temperature (°C)
- Minimum & Maximum temperature
- Humidity
- Cloud coverage
- Wind speed
- Real-time date and time
- Dynamic background images based on weather condition

It allows searching from a dataset of **275 predefined locations** with latitude and longitude set. The project also includes a **favorites feature**, enabling users to save and revisit preferred locations — stored in `localStorage`.

---

## ✨ Features

✅ Real-time weather data  
✅ Search across 275 popular cities  
✅ Favorite locations saved in localStorage  
✅ Dynamic weather-based background images  
✅ Live date and time display  
✅ Custom hook `useWeather` for API interaction  
✅ Graceful handling of internet disconnection with loader  
✅ Built with React Context API for global state  

---

## 🛠️ Tech Stack

- **Framework:** React (with Context API, useState, useEffect)
- **Build Tool:** Vite
- **Styling:** Tailwind CSS
- **State Management:** Context API & localStorage
- **Custom Hook:** `useWeather` for data fetching
- **Data Source:** OpenWeatherMap API
- **Location Dataset:** 275 locations (with lat/lon)

---

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/ziaulhoquepatwary/Weather-Dashboard.git
   cd Weather-Dashboard
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Create `.env` file**

   Inside the root folder, create a file named `.env` and add:

   ```
   VITE_WEATHER_API_KEY=your_openweather_api_key_here
   ```

   > ⚠️ The `.env` file is **.gitignored** and must be manually created. Without this, the project will not run.

   📘 Need help setting up the API key? See [**API_KEY_GUIDE.md**](./API_KEY_GUIDE.md)

4. **Run the app**
   ```bash
   npm run dev
   ```

5. Open your browser at:
   ```
   http://localhost:5173
   ```

---

## 🧭 Usage Guide

- Type any location name from the predefined list (275 cities) into the search bar.
- Click the ❤️ icon to mark/unmark as favorite.
- Favorite locations persist in your browser using localStorage.
- Background image and displayed data update according to the weather.
- If you're offline, a loading spinner will appear until the internet is restored.

---

## 📸 Screenshots

![Homepage View](./public/weather-deshboard-home-page.PNG)  
![Search Result](./public/weather-deshboard-search-page-1.PNG)  
![Favorites View](./public/weather-deshboard-fav-page-1.PNG)

---

## 🎬 Demo Video

Click the image below to watch the full demo on Vimeo:

[![Watch Demo](./public/weather-deshboard-home-page.PNG)](https://vimeo.com/1105562996)

---

## 🔗 Project Links

- 🔗 **GitHub Repository:** [https://github.com/ziaulhoquepatwary/Weather-Dashboard.git](https://github.com/ziaulhoquepatwary/Weather-Dashboard.git)
- 🌐 **Live Demo:** [https://weather-dashboard-three-iota.vercel.app/] (https://weather-dashboard-three-iota.vercel.app/)

---

## 🌍 Supported Locations

The app currently supports weather search for **275 predefined locations**.  
You can only search for these locations.

📄 See full list here: [SUPPORTED_LOCATIONS.md](./SUPPORTED_LOCATIONS.md)

---

## 🔮 Future Improvements

- Enable search for **any location** globally via geocoding API
- Add 5-day weather forecast
- Store favorites in backend with user authentication
- Add charts or visualizations (temperature, humidity over time)
- Convert to TypeScript for better scalability

---

## 📂 Folder Structure

```
src/
├── assets/
├── components/
│   ├── Header.jsx
│   ├── WeatherCard.jsx
│   └── ...
├── context/
│   └── weatherContext.jsx
├── hooks/
│   └── useWeather.js
│   └── useLocalStorage.js
├── data/
│   └── locations-data.js
├── provider/
│   └── WeatherProvider.js
├── utils/
│   └── date-utils.js
├── App.jsx
├── Page.jsx
└── main.jsx
```

---

## 🧠 Developer Notes

- ⚙️ Uses a custom hook (`useWeather`) to fetch and manage weather data
- 🌐 All requests use the **OpenWeatherMap API**
- 💾 Favorites are managed using `localStorage`
- 🧠 Uses React Context to provide global state for weather data and favorites
- 🛰️ Loader activates during API calls and network disconnections

---

## 👨‍💻 Author

**Ziaul Hoque Patwary**  
📧 Email: [**ziaul.dev@gmail.com**] 
🔗 GitHub: [ziaulhoquepatwary](https://github.com/ziaulhoquepatwary)

---

**Thanks for visiting the project! Feel free to star ⭐ the repo or contribute.**


# ⚡ WeatherPro - Advanced Weather Platform

<div align="center">

![WeatherPro Banner](https://img.shields.io/badge/WeatherPro-Advanced%20Weather%20Platform-blueviolet?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Open-Meteo API](https://img.shields.io/badge/Open--Meteo-API-orange?style=for-the-badge)

**A stunning, feature-rich weather application with advanced UI/UX and real-time weather data**

[Live Demo](#) • [Report Bug](https://github.com/vikashkumarsingh21/weatherpro/issues) • [Request Feature](https://github.com/vikashkumarsingh21/weatherpro/issues)

</div>

---

## 📸 Screenshots

<div align="center">
  <img src="screenshots/hero.png" alt="Hero Section" width="800"/>
  <p><i>Beautiful glassmorphism design with animated backgrounds</i></p>
</div>

<div align="center">
  <img src="screenshots/forecast.png" alt="Forecast Section" width="800"/>
  <p><i>Interactive 7-day forecast with hover effects</i></p>
</div>

---

## ✨ Features

### 🎨 **Premium UI/UX Design**
- **Glassmorphism Effects** - Modern frosted glass appearance with backdrop blur
- **Animated Gradient Background** - Dynamic color-shifting background
- **100 Twinkling Stars** - Atmospheric particle effects
- **Smooth Animations** - Bounce, float, pulse, and shimmer effects throughout
- **3D Hover Effects** - Interactive cards that respond to user interaction
- **Responsive Design** - Perfectly adapts to mobile, tablet, and desktop

### 🌤️ **Comprehensive Weather Data**
- **Current Weather** - Real-time temperature, conditions, and weather icon
- **Hourly Forecast** - 24-hour detailed weather timeline with scrollable interface
- **7-Day Forecast** - Weekly weather predictions with high/low temperatures
- **Detailed Metrics** - Wind speed, humidity, feels-like temperature, pressure
- **Sunrise/Sunset Times** - Daily sun schedule information
- **Air Quality Index** - Environmental air quality monitoring
- **Visibility Data** - Current visibility range information

### 🚀 **Advanced Functionality**
- **Smart City Search** - Search weather for any city worldwide
- **GPS Location Detection** - Automatic current location weather on page load
- **Temperature Unit Toggle** - Switch between Celsius and Fahrenheit
- **Smooth Scroll Navigation** - Navigate to sections seamlessly
- **Real-time Updates** - Live date and time display
- **Error Handling** - User-friendly error messages with animations
- **Loading States** - Beautiful loading screen with spinner animation

### ⚡ **Technical Highlights**
- **No API Key Required** - Uses free Open-Meteo API
- **Vanilla JavaScript** - Pure JS, no frameworks or dependencies
- **Optimized Performance** - Fast loading and smooth interactions
- **Clean Code Structure** - Well-organized and documented code
- **Cross-browser Compatible** - Works on all modern browsers

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| **HTML5** | Structure and semantic markup |
| **CSS3** | Advanced styling with animations and glassmorphism |
| **JavaScript (ES6+)** | Dynamic functionality and API interactions |
| **Open-Meteo API** | Weather data source |
| **Geocoding API** | Location search and coordinates |

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection for API calls
- Basic knowledge of HTML/CSS/JS (for customization)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/vikashkumarsingh21/weatherpro.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd weatherpro
   ```

3. **Open the application**
   ```bash
   # Simply open index.html in your browser
   # OR use a local server (recommended)
   
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (http-server)
   npx http-server
   
   # Using VS Code Live Server
   # Right-click index.html and select "Open with Live Server"
   ```

4. **Access the application**
   - Open your browser and go to `http://localhost:8000`
   - Or directly open `index.html` file

### Quick Start
1. The app automatically detects your location and shows weather data
2. Search for any city using the search bar
3. Click "Current Location" to refresh your location weather
4. Toggle between °C and °F using the navigation link
5. Explore hourly and 7-day forecasts

---

## 📂 Project Structure

```
weatherpro/
│
├── index.html              # Main HTML file
├── README.md               # Project documentation
├── screenshots/            # Screenshot images
│   ├── hero.png
│   ├── forecast.png
│   └── mobile.png
│
└── assets/                 # (Optional) Additional assets
    ├── favicon.ico
    └── logo.png
```

---

## 🎯 Key Components

### **Navigation Bar**
- Logo and branding
- Quick navigation links
- Temperature unit toggle

### **Search Section**
- City search input with autocomplete-ready design
- Search button with icon
- Current location GPS button

### **Hero Weather Panel**
- Large temperature display with animated icon
- City name and current date/time
- Weather description
- Key metrics (wind, humidity, feels-like, pressure)

### **Side Panel**
- 24-hour hourly forecast with scrollable timeline
- Air Quality Index with animated circular display

### **7-Day Forecast**
- Interactive forecast cards
- Daily weather icons and descriptions
- High/low temperature ranges
- Hover effects with shimmer animation

### **Additional Info Section**
- Sunrise and sunset times
- Visibility information
- Expandable details

---

## 🌐 API Reference

### Open-Meteo API
This project uses the free [Open-Meteo API](https://open-meteo.com/) for weather data.

**Endpoints Used:**
- **Weather Forecast**: `https://api.open-meteo.com/v1/forecast`
- **Geocoding**: `https://geocoding-api.open-meteo.com/v1/search`

**Parameters:**
- `latitude`, `longitude` - Location coordinates
- `current` - Current weather variables
- `hourly` - Hourly forecast data
- `daily` - Daily forecast data
- `timezone` - Automatic timezone detection

**No API key required!** ✨

---

## 🎨 Customization

### Change Color Scheme
Edit the gradient colors in the CSS:
```css
.animated-bg {
    background: linear-gradient(135deg, #1e3c72 0%, #2a5298 50%, #7e22ce 100%);
}
```

### Modify Animations
Adjust animation timings and effects:
```css
@keyframes gradientShift {
    0%, 100% { transform: translate(0, 0) scale(1); }
    50% { transform: translate(50px, 50px) scale(1.1); }
}
```

### Add More Weather Details
Extend the API call with additional parameters:
```javascript
const response = await fetch(
    `https://api.open-meteo.com/v1/forecast?latitude=${lat}&longitude=${lon}&current=temperature_2m,uv_index,cloud_cover`
);
```

---

## 📱 Responsive Breakpoints

| Device | Breakpoint | Layout |
|--------|------------|--------|
| Mobile | < 768px | Single column, stacked cards |
| Tablet | 768px - 1200px | Two columns, adjusted spacing |
| Desktop | > 1200px | Multi-column grid, full features |

---

## 🐛 Known Issues

- Air Quality Index displays static data (requires additional API integration)
- Visibility information is currently hardcoded
- Some weather codes may not have specific icons

---

## 🔮 Future Enhancements

- [ ] Add weather radar/map integration
- [ ] Implement weather alerts and warnings
- [ ] Add historical weather data charts
- [ ] Include pollen and UV index
- [ ] Add weather comparison between cities
- [ ] Implement favorite cities list
- [ ] Add weather widgets for embedding
- [ ] Multi-language support
- [ ] Dark/Light theme toggle
- [ ] Export weather data functionality
- [ ] Progressive Web App (PWA) support
- [ ] Push notifications for weather alerts

---

## 🤝 Contributing

Contributions are what make the open-source community amazing! Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Contribution Guidelines
- Follow the existing code style
- Write clear commit messages
- Update documentation as needed
- Test your changes thoroughly
- Add screenshots for UI changes

---

## 📝 License

Distributed under the MIT License. See `LICENSE` file for more information.

```
MIT License

Copyright (c) 2025 Vikash Kumar

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

## 👨‍💻 Author

**Vikash Kumar**

- GitHub: [@vikashkumarsingh21](https://github.com/vikashkumarsingh21)
- LinkedIn: [vikash kumar](https://www.linkedin.com/in/vikas-kumar-0803r/)
- Email: vk0102103@gmail.com
- Portfolio: [yourwebsite.com](https://portfolio-cb1t.onrender.com/)

---

## 🙏 Acknowledgments

- [Open-Meteo](https://open-meteo.com/) - Free weather API
- [Google Fonts](https://fonts.google.com/) - Inter font family
- Design inspiration from modern weather apps
- Icons and emojis from Unicode standard
- Community feedback and contributions

---

## 📊 Project Stats

![GitHub Stars](https://img.shields.io/github/stars/vikashkumarsingh21/weatherpro?style=social)
![GitHub Forks](https://img.shields.io/github/forks/vikashkumarsingh21/weatherpro?style=social)
![GitHub Issues](https://img.shields.io/github/issues/vikashkumarsingh21/weatherpro)
![GitHub Pull Requests](https://img.shields.io/github/issues-pr/vikashkumarsingh21/weatherpro)
![GitHub Last Commit](https://img.shields.io/github/last-commit/vikashkumarsingh21/weatherpro)

---

## 📞 Support

If you have any questions or need help, feel free to:
- Open an [issue](https://github.com/vikashkumarsingh21/weatherpro/issues)
- Email me at vk0102103@gmail.com


---

## ⭐ Star History

If you find this project useful, please consider giving it a star! ⭐

<div align="center">

**Made with ❤️ and JavaScript**

[⬆ Back to Top](#-weatherpro---advanced-weather-platform)

</div>

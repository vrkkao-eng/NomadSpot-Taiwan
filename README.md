# NomadSpot Taiwan ☕

>  A curated workspace discovery map for digital nomads in Taiwan. - 台灣數位遊牧咖啡廳探索地圖

---

## Overview

NomadSpot Taiwan is an interactive web application that helps digital nomads, remote workers, and café-hoppers discover the best café workspaces across Taiwan. It combines real-time weather and AQI data to help users find the ideal spot to settle in and get things done.

**Supported Language: English

---

## Features

- 🗺️ **Interactive Leaflet.js Map** — browse cafés by region with custom SVG map markers
- 🌤️ **Real-time Weather & AQI** — live environmental data per location via external APIs
- 🚲 **Real-time Youbike info** — live availability data per location via external APIs
- 🎨 **Nearby Attraction info** — nearby attraction data per location and automatized translation (from traditional Chinese to English) via external APIs
- ☕ **Café Detail Panel** — responsive drawer / bottom-sheet with photos, amenities, and contact info
- 📱 **Responsive Design** — two-page architecture optimised for both desktop and mobile

---

##  Project Structure

```
/NomadSpot-Taiwan
│
├── .gitignore
├── package.json                # Node.js dependencies & scripts
├── package-lock.json
├── server.js                   # Production Express server (Vercel)
├── vercel.json                 # Vercel deployment configuration
├── data/
│   └── cafes.json              # Curated café dataset (all locations & metadata)
├── public/                     # Static frontend assets served to browser
│   ├── index.html              # Landing / intro page
│   ├── map.html                # Main map application page
│   ├── map.js                  # Map logic — English version
│   ├── styles.css              # Global styles — English version
│   └── assets/
│       ├── favicon.svg
│       ├── cafe-images/        # Café photography (cafe-1.jpg … cafe-27.jpg)
│       └── icons/
│       └── icons/              # UI icons & region markers
│           ├── logo.svg
│           ├── NomadSpot TW.svg
│           ├── north.svg       # Region: North Taiwan
│           ├── central.svg     # Region: Central Taiwan
│           ├── south.svg       # Region: South Taiwan
│           ├── east.svg        # Region: East Taiwan
│           ├── bicycle2.svg
│           ├── clock.svg
│           ├── location.svg
│           ├── instagram.svg
│           ├── phone.svg
│           ├── star.svg
│           ├── rain.svg
│           └── wind.svg        # UI icons & region markers
│
└── scripts/
    └── verify-bff.mjs          # BFF (Backend-for-Frontend) verification script
---

##  License

This project is for personal and educational use. All café images and data are curated independently.

---

## Acknowledgements

Design by Shelly and Sophie.
Built with ☕ and 💻 by Lieselotte, Victor, Sophie, and Shelly.

> *Study near the mountains. Code by the beach. Explore night markets when you’re done. Discover our selection of work-friendly cafés across Taiwan, with live weather and bike availability, plus destination info to plan your next trip.*

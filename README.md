# NomadSpot Taiwan ☕

>  A curated workspace discovery map for digital nomads in Taiwan. - 台灣數位遊牧咖啡廳探索地圖

---

## Overview

NomadSpot Taiwan is an interactive, multilingual web application that helps digital nomads, remote workers, and café-hoppers discover the best café workspaces across Taiwan. It combines real-time weather and AQI data to help users find the ideal spot to settle in and get things done.

**Supported Languages  English

---

## Features

- 🗺️ **Interactive Leaflet.js Map** — browse cafés by city or region with custom SVG map markers
- 🌤️ **Real-time Weather & AQI** — live environmental data per location via external APIs
- 🖼️ **Café Detail Panel** — responsive drawer / bottom-sheet with photos, amenities, and contact info
- 📱 **Responsive Design** — two-page architecture optimised for both desktop and mobile
- 🎨 **Editorial Heritage Design System** — custom typography, palette, and iconography

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
│   │
│   └── assets/
│       ├── favicon.svg
│       ├── cafe-images/        # Café photography (cafe-1.jpg … cafe-27.jpg)
│       │
│       └── icons/              # UI icons & region markers
│           ├── logo.svg
│           ├── NomadSpot TW.svg
│           ├── north.svg       # Region: North Taiwan
│           ├── central.svg     # Region: Central Taiwan
│           ├── south.svg       # Region: South Taiwan
│           ├── east.svg        # Region: East Taiwan
│           ├── bicycle2.svg
│           ├── clock.svg / clock.png
│           ├── location.png
│           ├── instagram.png
│           ├── phone.png
│           ├── star.png
│           ├── rain.png
│           └── wind.png
│
└── scripts/
    └── verify-bff.mjs          # BFF (Backend-for-Frontend) verification script

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Map Engine | [Leaflet.js](https://leafletjs.com/) |
| Backend | [Express.js](https://expressjs.com/) (Node.js) |
| HTTP Client | Axios |
| Environment | dotenv |
| Deployment | [Vercel](https://vercel.com/) |
| Data | Static JSON (`data/cafes.json`) |

---

##  Getting Started

###  Prerequisites

- Node.js `>= 18.x`
- npm

### Installation

```bash
git clone https://github.com/<your-username>/NomadSpot-Taiwan.git
cd NomadSpot-Taiwan
npm install
```

###  Environment Variables

Create a `.env` file in the project root (see `.env` for reference):

```env
WEATHER_API_KEY=your_openweather_api_key
AQI_API_KEY=your_aqi_api_key
PORT=3000
```

## Scripts
| Script | Description |
|---|---|
| `node server.js` | Start production server |
| `node scripts/verify-bff.mjs` | Verify Backend-for-Frontend proxy routes |

---

##  License

This project is for personal and educational use. All café images and data are curated independently.

---

## Acknowledgements

Design by Shelly and Sophie.
Built with ☕ and 💻 by Lieselotte, Victor, Sophie, and Shelly.

> *Find your spot. Do your best work.*

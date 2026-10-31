# ☀️ HELIOGUARD — AI-Powered Solar Storm Intelligence

> **Planetary Protection System** — Real-time space weather monitoring,
> solar activity tracking, and Earth impact assessment.

![Status](https://img.shields.io/badge/status-v0.1.0_prototype-blue)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 🚀 What is HELIOGUARD?

HELIOGUARD is a modern space-weather monitoring and intelligence platform
that uses real-time data from NOAA's Space Weather Prediction Center (SWPC)
to monitor solar activity, geomagnetic storms, solar wind conditions, and
assess potential impacts on Earth and space infrastructure.

### Planned Features

| # | Feature | Status |
|---|---------|--------|
| 1 | Live Space Weather Dashboard | 🟡 In Progress |
| 2 | Solar Activity Monitoring | ⬜ Planned |
| 3 | Earth Impact Assessment | ⬜ Planned |
| 4 | AI Mission Scientist (Gemma) | ⬜ Planned |
| 5 | Solar Storm Simulator | ⬜ Planned |
| 6 | 3D Earth/Sun Visualisation | 🟡 In Progress |

---

## 📁 Project Structure

```
helioguard/
├── frontend/                # React + Vite + TypeScript
│   ├── src/
│   │   ├── components/      # React components
│   │   │   ├── Navbar.tsx         # Top navigation bar
│   │   │   ├── Dashboard.tsx      # Main dashboard layout
│   │   │   ├── StatusCard.tsx     # Metric display cards
│   │   │   ├── SolarVisual.tsx    # 3D Sun/Earth visual
│   │   │   ├── SolarWindChart.tsx # Solar wind chart
│   │   │   ├── AlertPanel.tsx     # Alerts panel
│   │   │   ├── ActivityFeed.tsx   # Activity timeline
│   │   │   └── StatusBar.tsx      # Bottom status bar
│   │   ├── App.tsx          # Root application component
│   │   ├── main.tsx         # Entry point
│   │   └── index.css        # Global styles + Tailwind
│   ├── index.html           # HTML template
│   ├── vite.config.ts       # Vite configuration
│   ├── package.json         # Frontend dependencies
│   └── tsconfig.json        # TypeScript configuration
├── backend/                 # Python FastAPI
│   ├── main.py              # API server
│   └── requirements.txt     # Python dependencies
├── .gitignore
├── .env.example
└── README.md
```

---

## 🛠️ Getting Started

### Prerequisites

Make sure you have these installed:

- **Node.js** (v18 or later) — [Download](https://nodejs.org/)
- **Python** (3.10 or later) — [Download](https://python.org/)
- **Git** — [Download](https://git-scm.com/)

### 1. Start the Frontend

Open a terminal and run:

```bash
cd helioguard/frontend
npm install          # Install dependencies (only needed first time)
npm run dev          # Start the development server
```

The frontend will be available at: **http://localhost:5173**

### 2. Start the Backend

Open a **second terminal** and run:

```bash
cd helioguard/backend

# Create a virtual environment (recommended, first time only)
python -m venv venv

# Activate the virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Start the API server
uvicorn main:app --reload --port 8000
```

The backend API will be available at: **http://localhost:8000**

Interactive API docs at: **http://localhost:8000/docs**

---

## 🔗 Local URLs

| Service | URL | Description |
|---------|-----|-------------|
| Frontend | http://localhost:5173 | Main HELIOGUARD dashboard |
| Backend API | http://localhost:8000 | FastAPI server |
| API Docs | http://localhost:8000/docs | Interactive Swagger docs |
| Health Check | http://localhost:8000/api/health | Server health endpoint |

---

## 🎨 Tech Stack

- **Frontend**: React + TypeScript + Vite
- **Styling**: Tailwind CSS
- **3D Graphics**: Three.js / React Three Fiber
- **Charts**: Recharts
- **Backend**: Python + FastAPI
- **Data Source**: NOAA SWPC (planned)
- **AI**: Google Gemma (planned)

---

## ⚠️ Current Status

This is **v0.1.0** — the initial project scaffold with:
- ✅ Project structure and configuration
- ✅ Beautiful space-themed dashboard UI
- ✅ 3D Sun/Earth visual placeholder
- ✅ Dashboard cards with DEMO data
- ✅ Solar wind chart placeholder
- ✅ Alert and activity panels
- ✅ FastAPI backend with health check
- ⬜ Real NOAA data integration (next step)

All data currently shown is **DEMO placeholder data**.

---

## 📜 License

MIT License — free to use, modify, and distribute.

# VayuGuard AI — Urban Air Quality & Winter Smog Assistant

A GenAI-powered civic-tech web application designed to help Indian families, commuters, and Resident Welfare Associations (RWAs) navigate severe winter smog and urban air pollution with localized, actionable routines and quantified environmental/health impact metrics.

## Live Demo (GitHub Pages)
Once uploaded to your GitHub repository, enable **Settings → Pages → Deploy from branch (`main` / `root`)** to generate a shareable public URL (`https://<your-username>.github.io/<repo-name>/`).

## Repository Structure
```text
├── INDEX.HTML         # Complete self-contained application (UI, CSS, JS, Charts, Voice AI, Unit Tests)
├── REQUIREMENTS.MD    # Functional, non-functional, CPCB domain, and accessibility specifications
├── README.MD          # Project overview, architecture, setup, and GitHub Pages deployment guide
└── TASKS.MD           # Development milestones, sprint checklist, and verification status
```

## Key Features
- **CPCB Indian AQI Dashboard & Smog Spike Simulator**: Tracks 8 major Indian metros (Delhi NCR, Hyderabad, Mumbai, Bengaluru, Kolkata, Chennai, Pune, Ahmedabad) across all 6 NAAQS pollutants (`PM2.5`, `PM10`, `NO₂`, `SO₂`, `CO`, `O₃`) with a real-time AQI stress-test slider (`25–500`).
- **GenAI + Deterministic Offline Advisor**: Generates personalized low-emission routines, Indian indoor air quality hacks (damp *pocha* mopping vs. dry sweeping, *tadka* exhaust timing, ₹1,500 DIY MERV-13/HEPA box fan, afternoon inversion ventilation window), and community RWA interventions. Works instantly offline or connects to **Google Gemini (`gemini-2.0-flash`)** when an API key is supplied.
- **Quantified Impact Calculator**: Shows exact daily `CO₂` prevented (`kg/day`), personal `PM2.5` intake reduction (`%`), and daily fuel/health cost savings (`₹/day`).
- **Interactive Data Visualizations (`Chart.js`)**:
  - 24-Hour Winter Inversion Diurnal `PM2.5` Trend
  - Baseline vs. Protected Personal `PM2.5` Exposure Comparison
  - 8-City Indian Metro AQI Bar Comparison
- **Web Speech API Voice Assistant**: Spoken `en-IN` AQI briefings and voice-activated Q&A.
- **Persistence, Export & Quality Assurance**: `localStorage` session history, one-click CSV report download, Dark/Light mode, WCAG AA keyboard accessibility, and an integrated 8-test in-browser unit test runner.

## Quick Start
1. Clone or download this repository.
2. Open `INDEX.HTML` directly in any modern browser (Chrome, Edge, Safari, Firefox) — no build step or backend server required.
3. Click **🧪 Run Unit Tests** inside the dashboard to verify all core logic assertions.

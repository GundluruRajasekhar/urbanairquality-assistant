# Project Execution & Verification Tasks — VayuGuard AI

## Phase 1: Architecture & Domain Modeling
- [x] Define CPCB 6-tier AQI breakpoints (`0–50`, `51–100`, `101–200`, `201–300`, `301–400`, `401–500`) and health advisories.
- [x] Compile baseline 6-pollutant and 24-hour diurnal inversion profiles for 8 Indian cities (Delhi NCR, Hyderabad, Mumbai, Bengaluru, Kolkata, Chennai, Pune, Ahmedabad).
- [x] Design quantified impact formulas for `CO₂` reduction (`kg/day`), personal `PM2.5` exposure drop (`%`), and fuel/health savings (`₹/day`).

## Phase 2: Core UI, Visualizations & GenAI Engine
- [x] Build responsive semantic HTML5 layout with Light/Dark theme switcher in `INDEX.HTML`.
- [x] Implement interactive `Chart.js` visualizations (24-Hour Inversion Trend, Baseline vs. Protected Exposure, 8-City Comparison).
- [x] Implement hybrid GenAI advisor supporting both optional Gemini API key execution and instant offline Indian household recommendations.
- [x] Add Smog Spike Simulator slider (`25–500`) for real-time scenario testing.

## Phase 3: Accessibility, Voice, Storage & Testing
- [x] Integrate Web Speech API (`speechSynthesis` `en-IN` briefing + `SpeechRecognition` voice queries).
- [x] Implement `localStorage` assessment history table and one-click CSV report export.
- [x] Add in-browser 8-assertion automated unit test suite (`🧪 Run Unit Tests`).
- [x] Complete repository documentation (`README.MD`, `REQUIREMENTS.MD`, `TASKS.MD`) for GitHub Pages deployment.

## Phase 4: GitHub Deployment Checklist
- [ ] Create a new public repository on GitHub (e.g., `vayuguard-ai`).
- [ ] Upload `INDEX.HTML` (also save/rename a lowercase copy as `index.html` if needed by GitHub Pages), `README.MD`, `REQUIREMENTS.MD`, and `TASKS.MD`.
- [ ] Enable **Settings → Pages → Source: Deploy from a branch (`main` / `/root`)**.
- [ ] Share the generated `github.io` link for live judging and community testing.

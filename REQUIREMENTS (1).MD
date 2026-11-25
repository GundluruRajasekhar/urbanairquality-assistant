# System & Product Requirements — VayuGuard AI

## 1. Problem Statement
During winter months across North and Central India, meteorological temperature inversions combine with vehicular exhaust, construction dust, and biomass burning to push Air Quality Index (AQI) levels into **Very Poor (301–400)** and **Severe (401–500)** categories. Families lack hyper-local, actionable guidance that connects daily household/commute choices to measurable reductions in personal `PM2.5` intake and carbon emissions.

## 2. Functional Requirements
| ID | Requirement | Description | Priority |
| :--- | :--- | :--- | :--- |
| **FR-01** | **CPCB AQI Classification** | Classify AQI values (0–500) strictly according to India's Central Pollution Control Board (CPCB) 6-band color and health advisory scale (`Good`, `Satisfactory`, `Moderate`, `Poor`, `Very Poor`, `Severe`). | Must Have |
| **FR-02** | **Multi-City Indian Coverage** | Provide baseline pollutant profiles (`PM2.5`, `PM10`, `NO₂`, `SO₂`, `CO`, `O₃`) and 24-hour diurnal curves for 8 major Indian cities. | Must Have |
| **FR-03** | **Interactive Smog Simulator** | Allow users and hackathon judges to simulate AQI spikes (`25–500`) via a slider and observe real-time updates across charts and advisories. | Must Have |
| **FR-04** | **Tailored Lifestyle & IAQ Engine** | Generate recommendations customized by household type (kids/elders, commuter, senior, RWA), commute mode, and home ventilation setup. | Must Have |
| **FR-05** | **Hybrid GenAI + Offline Execution** | Support optional live Google Gemini API calls while guaranteeing zero-latency offline fallback recommendations without requiring an API key. | Must Have |
| **FR-06** | **Quantified Choice Impact** | Display concrete daily savings in `CO₂` (`kg`), personal `PM2.5` intake (`%`), and Indian Rupees (`₹/day`). | Must Have |
| **FR-07** | **Voice Briefing & Query** | Integrate browser `speechSynthesis` (`en-IN`) and `SpeechRecognition` for hands-free accessibility. | Should Have |
| **FR-08** | **Data Persistence & CSV Export** | Persist recent assessments in `localStorage` and allow one-click export of city AQI metrics to `.csv`. | Should Have |

## 3. Non-Functional Requirements
- **NFR-01 (Zero-Backend Portability)**: Must run cleanly as static files on GitHub Pages without Node.js build pipelines or server dependencies.
- **NFR-02 (Accessibility — WCAG 2.1 AA)**: Includes skip-to-content navigation, semantic landmarks, `aria-live` regions, high-contrast Dark/Light themes, and visible focus rings.
- **NFR-03 (Security & Resilience)**: All dynamic DOM insertions sanitize strings against XSS; `localStorage` and network calls degrade gracefully on failure.
- **NFR-04 (Responsive Design)**: Fluid CSS Grid layout supporting mobile viewports (`360px+`), tablets, and wide desktop screens.

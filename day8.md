# Day 8 — 🌍 Personal Environmental Health Analyzer

## What I Built

Today I built a **Personal Environmental Health Analyzer** — a fully interactive, single-file HTML dashboard that pulls together real-world air and water quality data for 20 major cities across 6 continents and turns it into a personalized health intelligence tool.

The dashboard is built entirely in vanilla HTML, CSS, and JavaScript with Chart.js for visualizations. No frameworks, no backend — just one `index.html` you can open anywhere.

### Core Features

- **20 Cities Analyzed** — Delhi, Mumbai, Lahore, Dhaka, Beijing, Cairo, Jakarta, Bangkok, Lagos, Karachi, Los Angeles, London, Paris, New York, Sydney, Tokyo, Stockholm, Zurich, Vancouver, and Wellington
- **Real 2026 AQI Data** — sourced from IQAir World Air Quality Report 2026, WHO guidelines, and US EPA AQI standards
- **5 Interactive Charts** — AQI comparison, PM2.5 with WHO guideline overlay, PM10 with WHO guideline overlay, AQI distribution donut, and city environmental ranking
- **Live Filters** — city selector, AQI category filter (Good → Severe), pollutant switcher (AQI / PM2.5 / PM10), and region filter (Asia / West / Other) — all charts and cards update in real time
- **City Detail Cards** — color-coded AQI badges, animated fill bars, and triple scores (Air Score, Water Score, Overall Score) for every city
- **Deep Dive Panel** with 3 tabs:
  - 🫁 **Air Health** — impact on lungs, sleep, energy, exercise performance, cardiovascular health, and long-term risk
  - 💧 **Water & Skin** — hair fall risk, hair dryness, scalp health, skin dryness, acne, and sensitive skin — all driven by water TDS and hardness data
  - 💡 **Personalized Recommendations** — daily actions, indoor air improvements, water treatment suggestions, hair/scalp care, skincare, and outdoor exercise guidance
- **Environmental Report Card** — A–F grades for Air Quality, Water Quality, Hair Risk, and Skin Risk with animated score bars
- **Insights Panel** — top 3 cleanest cities, top 3 most polluted, biggest anomaly, and most surprising observation

---

## What I Observed

### The Data Gap Is Shocking
The AQI spread across 20 cities is 164 points — Wellington sits at **AQI 8** (essentially pristine) while Lahore hits **172** (Poor/Unhealthy). That's not a small difference — it represents a fundamentally different biological experience for the people living in those cities every single day.

### PM2.5 Is The Real Villain
Every city above AQI 100 exceeded the WHO annual PM2.5 guideline of 5 μg/m³ by a factor of 10–20×. Delhi at 99.6 μg/m³ annual average is nearly **20× the WHO guideline**. The WHO number isn't aspirational — it's the threshold below which chronic disease risk starts dropping meaningfully.

### Water Quality Tracks Air Quality (Mostly)
Cities with bad air tend to also have bad water — hard, high-TDS water with scores below 40/100. The exception is Tokyo, which has excellent water (score: 90) despite moderate air pollution. This matters because the combined effect of bad air AND hard water on skin and hair is multiplicative, not additive.

### Air Pollution Is a Personal Health Problem, Not Just an Environmental One
Building the health impact engine made this visceral. PM2.5 doesn't just sit in your lungs — it enters your bloodstream, disrupts sleep architecture, reduces cognitive performance, and when combined with hard water, creates a cascade of skin and hair issues most people never trace back to their environment. The tool makes those invisible connections visible.

### The Cleanest Cities All Share One Thing
Stockholm (AQI 12), Zurich (AQI 18), Vancouver (AQI 22), Wellington (AQI 8) — all have aggressive environmental regulation, low car dependency or strong EV adoption, and high green cover. Clean air is a policy outcome, not a geographic accident.

### Responsive Design in a Single File Is Underrated
The entire dashboard — dark theme, animated grid background, 5 charts, tab panels, filter system, report card — lives in one HTML file under 600 lines. No build tools, no node_modules, no deployment pipeline. It opens instantly in any browser. There's something powerful about that simplicity.

---

## Tech Stack

| Layer | Tool |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox, animations) |
| Charts | Chart.js 4.4.1 via CDN |
| Typography | Syne + Space Grotesk (Google Fonts) |
| Data | IQAir 2026, WHO, US EPA AQI Standards |
| Output | Single `.html` file — zero dependencies |

---

## Key Metrics From the Analysis

| Metric | Value |
|---|---|
| Cities Analyzed | 20 |
| Average AQI | ~97 (Moderate) |
| Highest AQI | Lahore — 172 |
| Lowest AQI | Wellington — 8 |
| Cities Exceeding WHO PM2.5 | 12 out of 20 |
| Best Water Quality | Wellington — 97/100 |
| Worst Water Quality | Lagos — 28/100 |

---

## What's Next

- Connect to a live AQI API (IQAir or WAQI) so data updates automatically
- Add historical trend lines to show improvement/deterioration over time
- Geolocation-based auto-detection of the user's city
- Export report card as a shareable image or PDF

---

*Built with Claude · Data: IQAir World Air Quality Report 2026, WHO Environmental Health Guidelines, US EPA AQI Standards*

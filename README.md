# 🌾 AgriVision AI

### Smart Agricultural Market Intelligence System
**An AI-powered Decision Support System for Indian farmers — not just price prediction, but an actionable sell/wait recommendation with an exact rupee profit figure.**

Built for **Smart Kopargaon Hackathon (SKH)** by **Team The Elite Four**
Problem Statement ID: `skh005` | Theme: Agriculture | Category: Software

---

## 🚩 The Problem

- Farmers in India don't know which mandi offers the best price for their crop.
- They can't predict future prices, so they often sell at the wrong time.
- High transportation costs and guesswork-based decisions shrink already-thin profit margins.
- These compounding pressures are a contributing factor in farmer distress across India.

## 💡 Our Solution

AgriVision AI analyzes historical mandi prices, seasonal/festival demand patterns, and transport costs to answer one question farmers actually care about:

> **"Should I sell today, or wait? And which mandi should I go to?"**

Instead of a dashboard full of charts, the system outputs one clear recommendation — **SELL NOW** or **WAIT ~X DAYS** — backed by a real ₹ profit number, the best mandi to sell at, and the weather/seasonal reasoning behind the call.

## ✨ Key Features

- 📊 **30-day price trend comparison** across multiple mandis
- 🤖 **AI-style decision engine** — combines price trend, seasonality, and transport cost into one actionable call
- 📍 **Best Mandi recommendation** — accounts for distance and transport cost, not just headline price
- 🌦️ **Weather & seasonal reasoning** — explains *why* the recommendation was made
- 🪜 **Mandi comparison ladder** — all nearby mandis ranked by net profit
- 🌐 **Multilingual** — English, Hindi, and Marathi support
- 👨‍🌾 **Farmer login & dashboard** — simple, accessible interface

## 🛠️ Tech Stack (Planned Production Architecture)

| Layer | Technology |
|---|---|
| Frontend | Flutter |
| Backend | Python (FastAPI) |
| Database | PostgreSQL |
| AI/ML | XGBoost, Prophet, Scikit-learn |
| Maps | Google Maps API |
| Weather | OpenWeather API |
| Market Data | Agmarknet, data.gov.in, eNAM |
| Notifications | Firebase Cloud Messaging |
| Auth | JWT |
| Multilingual | Google Translate API |

## 🧪 Current Prototype

This repository includes a **working interactive prototype** (`agrivision_prototype.html`) that demonstrates the full decision-support flow end-to-end — crop selection, price trend visualization, mandi comparison, and the AI recommendation engine — running on a **demo dataset** modeled on real Agmarknet price patterns.

> ⚠️ **Note on data:** The prototype currently runs on a synthetic demo dataset (30 days × 3 crops × 3 mandis) modeled on real Agmarknet price behavior, since live data collection during the hackathon window was limited. The decision engine — trend analysis, transport-cost-adjusted profit calculation, and sell/wait logic — is fully functional and built to plug directly into live Agmarknet/eNAM/data.gov.in feeds without any architectural changes.

### Run it locally
Just download `agrivision_prototype.html` and open it in any browser — no installation or server required.

### Vedio Presentation Link : https://youtu.be/1yGpw6NA98E

## 📈 Feasibility & Impact

- Uses free, official government datasets (Agmarknet, data.gov.in)
- Can be adopted by FPOs (Farmer Producer Organisations) and state agriculture departments
- Scalable across crops and mandis nationwide
- Directly targets farmer profit loss from information asymmetry and high transport costs

## 📚 Research & References

- [Agmarknet](https://agmarknet.gov.in/home) — historical & daily mandi price data
- [data.gov.in](https://data.gov.in/) — government agriculture & commodity datasets
- [NABARD](https://www.nabard.org/) — research on agriculture, rural development, and AI applications in farming

## 👥 Team — The Elite Four

Team ID: `8K5YVT`

---

*Built with ❤️ for Indian farmers.*

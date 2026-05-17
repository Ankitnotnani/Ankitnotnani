# Ankit Notnani

> AI/ML undergrad building real systems — not just notebooks.
> Grand Finalist at NASA Space Apps 2025 & Smart India Hackathon 2025.

---

## About

I'm a third-year CSE (AI & ML) student at UPES Dehradun who builds things end-to-end — from edge AI on ESP32 and Raspberry Pi to NLP-powered web platforms to NASA Earth data apps. I've led teams at two of India's biggest hackathons and shipped real products under pressure. I care about clean architecture, useful AI, and code that actually solves something.

---

## Featured Projects

### ChronoClime — Hyper-Local Weather Intelligence App &nbsp; `NASA Space Apps 2025 — Grand Finalist`

A personalised weather app that goes beyond standard forecasts. Uses the **ACIS (Activity-Centric Impact Score)** — a custom 1–10 risk metric — to tell you whether a day is a 9/10 for cycling or a 3/10 for a picnic, and why. Includes an **Optimal Day Finder** that automatically identifies your best window across the forecast range.

**What makes it different:** Standard weather apps give you temperature and precipitation. ChronoClime fuses temperature, wind, humidity, UV, and AQI into a single activity-specific score, then surfaces the best day automatically. Includes an optional **ESP8266 IoT hardware gateway** for GPS-based location input and an **AI weather chatbot** for context-aware queries.

**My contributions:** Designed and implemented the ACIS scoring algorithm (the core differentiator), built the Activity Planner component, integrated the OpenWeatherMap API pipeline, developed the ESP8266 IoT gateway integration, and built the AI chatbot service.

**Architecture:** React 18 + TypeScript + Vite frontend · OpenWeatherMap API · Supabase · Leaflet maps · ESP8266 NodeMCU (Arduino firmware) · Google Apps Script sync

`React` `TypeScript` `Vite` `Tailwind CSS` `Framer Motion` `Supabase` `Leaflet` `ESP8266` `Arduino` `FastAPI`

🔗 [Repository](https://github.com/Ankitnotnani/ChronoClime)

---

### KASA — AI-Powered Laser QR Marking System &nbsp; `SIH 2025 — Grand Finalist`

Built for Indian Railways. An AI-powered lifecycle traceability system that assigns every track component a unique laser-etched QR identity. Served as **Software Lead**, owning the full AI ecosystem.

**What I built:** React frontend for field engineers to scan QR-marked components and retrieve complete maintenance history; AI analytics dashboard (Python/Dash/Plotly) with failure-rate visualisations, component lifespan forecasting by zone, and warranty alerts; cloud backend (Firebase/AWS) with REST APIs syncing bidirectionally to Indian Railways' UDM and TMS portals.

`Raspberry Pi` `Coral Edge TPU` `MobileNetV3` `React` `Firebase` `AWS` `Python` `Dash` `Plotly` `REST APIs`

---

### IDEACT — Intelligent SDG-Oriented Hackathon Advisor &nbsp; `Minor Project | UPES 2025–26`

A web-based AI platform that takes a hackathon problem statement, maps it to the relevant UN Sustainable Development Goals using NLP, and outputs structured project ideas with a full week-by-week execution roadmap.

**What it does:**
1. Preprocesses input — tokenization, stopword removal, lemmatization
2. Extracts top keywords using term frequency
3. Classifies against all 17 UN SDGs using a trained Logistic Regression model
4. Finds similar problems from a curated hackathon dataset via cosine similarity
5. Generates 1–5 project ideas with features, tech stack, SDG alignment, and India scheme fit
6. Builds a configurable 1–12 week execution roadmap

**Architecture:** Single-file React frontend → FastAPI REST API (6 endpoints) → Scikit-learn NLP pipeline (TF-IDF + Logistic Regression) + NLTK preprocessing · PostgreSQL + MongoDB data layer

**Team:** Ankit Notnani (AI/ML & Backend) · Abhishree Panwar (Data & Research) · Chaitanya Gaur (Frontend) · Kshaunish Singh (Backend & APIs)
**Mentor:** Prof. Aryan Gupta, Dept. of CSE, UPES

`Python` `FastAPI` `Scikit-learn` `NLTK` `TF-IDF` `React` `PostgreSQL` `MongoDB` `NLP` `REST APIs`

🔗 [Repository](https://github.com/Ankitnotnani/IDEACT)

---

### SwipeShop — Swipe-Based E-Commerce App

A Tinder-style mobile-first shopping app — swipe right to wishlist, swipe up to cart, swipe left to skip. Built with React + TypeScript + Capacitor for native iOS deployment.

**What makes it different:** Most e-commerce apps overwhelm users with cluttered grids. SwipeShop presents one product at a time with gesture-driven decisions — faster, more engaging, built mobile-first. Works with both touch (mobile) and mouse drag (desktop).

**My contributions:** Built the ProductCard swipe engine — touch and mouse gesture detection, directional swipe logic (left/right/up), overlay animations, and double-tap support. Developed CategoryTabs component and real-time search filtering. Assembled the full product catalog and handled UI polish across all components.

| Gesture | Action |
|---|---|
| Swipe Right → | Add to Wishlist |
| Swipe Up ↑ | Add to Cart |
| Swipe Left ← | Skip product |
| Double Tap | Add to Wishlist |

**Architecture:** React 18 + TypeScript + Vite · shadcn/ui · Tailwind CSS · React Context + useReducer · React Router v6 · TanStack Query · Capacitor (iOS)

`React` `TypeScript` `Vite` `shadcn/ui` `Tailwind CSS` `Capacitor` `React Query` `iOS`

🔗 [Repository](https://github.com/Ankitnotnani/SwipeShop)

---

### SIMM — Smart Industrial Machine Monitoring & Predictive Maintenance &nbsp; `Industry 4.0`

An edge AI system for predicting machinery failures before they occur — without needing historical failure data. Three-layer architecture: Edge DSP on ESP32 → Unsupervised AI Gateway → 3D Digital Twin dashboard.

**What makes it different:** Traditional IoT systems flood the cloud with raw sensor data. SIMM runs hardware-accelerated FFT directly on the ESP32, transmitting only dominant frequency and magnitude — reducing network payload by over 90%. The AI layer uses an Isolation Forest model that learns the machine's healthy baseline and flags anomalies without labelled failure data.

**My contributions:** Built the React frontend and 3D Digital Twin dashboard (App.jsx) — component structure, live telemetry graphs with Recharts, and real-time state updates. Helped develop the FastAPI backend — API routes, CORS, and SSE streaming for live data push. Assisted with the CSV data pipeline integrating PySerial logger output with backend processing.

**Architecture:** ESP32 firmware (C++/Arduino, hardware FFT) → PySerial CSV logger → FastAPI SSE backend → React Three Fiber 3D dashboard · Isolation Forest anomaly detection (Scikit-learn) · Monitors 6 machines simultaneously

**Team:** Kushagra Agarwal (Project Lead — hardware, firmware, AI) · Ankit Notnani (Frontend, backend, data pipeline)
*Guided by Dr. Ayush Agrawal.*

`ESP32` `Arduino` `FFT` `Python` `FastAPI` `Scikit-learn` `Isolation Forest` `React` `React Three Fiber` `WebGL` `Recharts` `Pandas`

🔗 [Repository](https://github.com/Ankitnotnani/SIMM)

---

### ExamHub — Microservices Exam Platform

Online exam system with JWT auth, service discovery, and an API gateway built on Spring Cloud. 5 independently deployable services communicating via REST.

`Spring Boot` `Spring Cloud` `Eureka` `JWT` `MySQL` `React`

---

### ArthSahayak — Personal Finance Companion App

Expense tracking, live market updates, and investment learning modules — built to make financial literacy accessible to young users through a data-driven interface.

`Python` `Financial APIs` `Data Analytics`

---

## Skills

**Languages:** Java · Python · C · JavaScript · TypeScript

**AI / ML:** Scikit-learn · TensorFlow · PyTorch · NumPy · Pandas · Isolation Forest · NLP (NLTK, TF-IDF)

**Web & Frontend:** React · Vite · Tailwind CSS · Framer Motion · React Three Fiber · shadcn/ui · HTML · CSS

**Backend & APIs:** FastAPI · Flask · Spring Boot · Spring Cloud · REST APIs · SSE · JWT

**Databases:** PostgreSQL · MySQL · MongoDB · Firebase · Supabase

**Hardware & Edge:** Raspberry Pi · ESP32 · Coral Edge TPU · Arduino · MobileNetV3 · ESP8266

**DevOps & Tools:** Git · GitHub · Docker · AWS · Wireshark · Kali Linux

---

## Achievements

- Grand Finalist — **NASA Space Apps Challenge 2025** ("Will It Rain On My Parade?" — ChronoClime)
- Grand Finalist — **Smart India Hackathon 2025** (SIH25021 — Team KASA, UPES representative)
- Minor Project — **IDEACT**, AI-powered SDG hackathon advisor, UPES Dept. of CSE (2025–26)
- Internship — **Binary Keeda Education Pvt. Ltd.** · Tech & Social Media — drove 50% audience engagement growth in 2 months (Jun–Aug 2025)
- Internship — **Chhanv Foundation** · Supporting acid attack survivors — field campaigns, awareness sessions, Sheroes Hangout Cafe (Jun–Jul 2024)

---

## Positions of Responsibility

- Associate Secretary — Avishkarnam, The Literary Club of UPES (2023–Present)
- Anchor & Host — UURJA / Spandan / Ukti (large-scale UPES events, thousands of attendees)
- Former PR Head — Pratibimb Photography Club, UPES (2023–2024)

---

## Currently

Actively looking for **internships & collaborations** in backend, AI/ML, or full-stack roles.
Also happy to contribute to interesting open-source projects. If you're building something ambitious, let's talk.

---

## Get in Touch

- 📧 Email: [ankitnotnani6497@gmail.com](mailto:ankitnotnani6497@gmail.com)
- 💼 LinkedIn: [linkedin.com/in/ankit-notnani](https://www.linkedin.com/in/ankit-notnani/)
- 🐙 GitHub: [github.com/Ankitnotnani](https://github.com/Ankitnotnani)
- Response time: usually within 24 hours.

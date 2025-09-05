# 🟦⚡ InteliGuard: Predictive Maintenance and Automation System

<p align="center">
  <img src="https://skillicons.dev/icons?i=react,tailwind,unity,python,tensorflow,fastapi,docker,github,opencv,linux&perline=6" alt="Tech stack icons" />
</p>

---

## Overview

InteliGuard is a cyberpunk-themed Industry 4.0 unified dashboard for predictive maintenance and factory automation. It merges real-time sensor visualization, AI-powered safety & anomaly detection, AR digital twin, and Remaining Useful Life (RUL) prediction into a sleek, interactive platform for smart manufacturing.

---

## Features

- **Real-time Monitoring:** Motor sensors (frequency, voltage, current, RPM, temperature), VFD controller, Mitsubishi PLC, ESP32 Edge AI.
- **Industrial IoT:** MQTT Sparkplug B gateway, InfluxDB time-series database.
- **AI-Powered:** YOLOv8 webcam PPE detection, edge anomaly alerts, RUL prediction with CNN-GRU.
- **AR Digital Twin:** Unity 3D model synchronized with live OPC CSV data.
- **Interactive Cyberpunk UI:** Neon animated data flows, node modals, safety alerts.
- **Webcam Safety:** Detect helmets, gloves, vests, shoes; trigger safety stop simulation.

---

## Project Structure

src/
├── components/
│   ├── Dashboard.jsx
│   ├── Header.jsx
│   ├── SystemFlow.jsx
│   ├── SystemNode.jsx
│   ├── FlowConnection.jsx
│   ├── StatusPanel.jsx
│   └── NodeModal.jsx
├── App.jsx
├── main.jsx
├── index.css
└── App.css

---

## Tech Stack

| Technology | Purpose             |
|------------|---------------------|
| React.js   | Frontend UI         |
| Vite       | Dev Server          |
| TailwindCSS| Styling             |
| Framer Motion | Animations        |
| Recharts   | Charts              |
| Lucide     | Icons               |
| FastAPI    | Backend API & WebSocket |
| Unity3D    | AR Digital Twin     |
| YOLOv8     | PPE detection       |
| OpenCV     | Computer Vision     |
| InfluxDB   | Time-series DB      |
| Docker     | Containerization    |
| Linux      | Hosting             |

---

## Installation & Setup

### 1. Clone repository

git clone https://github.com/<your-org>/InteliGuard.git
cd InteliGuard

### 2. Frontend setup
cd frontend
npm install
npm run dev

- Access at `http://localhost:3000`
- Add nodes: modify `SystemFlow.jsx` and `NodeModal.jsx`
- Add images: place in `public/images/`
- Customize colors in `tailwind.config.js`

### 3. Backend setup

cd ../backend
pip install -r requirements.txt
uvicorn main:app --reload


- REST API for sensor data and AI models
- MQTT broker and InfluxDB integration

### 4. Unity Digital Twin

- Open `/digital-twin` in Unity
- Assign CSV data in `DigitalTwinController.csvFile`
- Assign motor/shaft/servo 3D models and UI text fields
- Press Play to run synchronized 3D visualization

### 5. YOLOv8 PPE Detection

cd ../ppe-detection
pip install -r requirements.txt
python cvdetection.py


- Place YOLOv8 `.pt` model in `model/` folder
- Webcam detects PPE and triggers safety alerts

---

## Usage

- Click dashboard nodes for detailed real-time data modals
- Observe neon animated data flows
- Activate PPE detection for live safety monitoring
- Monitor motor sensor streams, anomaly counts, AR twin model
- Use RUL dashboard for predictive maintenance decisions

---

## Browser Compatibility

- Chrome/Chromium (recommended)
- Firefox, Safari, Edge  
*Note: Webcam uses HTTPS in production*

---

## License

[MIT License](LICENSE)

---

## Contributions

Pull requests, issues, and feedback welcome!

---

<p align="center">
  <img src="https://skillicons.dev/icons?i=react,fastapi,python,unity,tailwind,opencv,tensorflow,pytorch,docker,github,linux,git" alt="Tech stack icons" />
</p>

---

Thank you for using **InteliGuard** — your all-in-one cyberpunk predictive maintenance and automation hub!


🔥 Forest Fire Risk Prediction System (Live Map + Weather + NASA FIRMS)
This project predicts and visualizes forest fire risk using live weather data, simulated NDVI vegetation grids, and optionally integrates NASA FIRMS satellite fire detection. Users can input any location (latitude & longitude), view a real-time interactive map showing fire risk zones, and download results for further analysis.

📌 Key Features
🌍 Interactive Map with fire risk zones (green = safe, red = high risk)

📡 Live weather data from OpenWeatherMap API

🌿 NDVI-based vegetation simulation

🛰️ Optionally integrates NASA FIRMS VIIRS fire data

📈 Fire risk calculated using a Random Forest ML model

📦 Exportable CSV report and HTML map

🧠 Realistic environmental factors: temperature, humidity, wind, slope, elevation, aspect

📍 Custom location input for user-defined simulation areas

🧠 Opportunity & Problem Solved
🔎 How is it different from existing systems?
Most systems only display fire alerts; they don't predict potential fire risk zones ahead of time.

We simulate environmental + terrain conditions to assess risk before an actual fire happens.

✅ How does it solve the problem?
Gives early warning visibility into high-risk areas

Helps forest departments or decision-makers take preventive action

Allows custom simulations for any location worldwide

💡 USP (Unique Selling Point)
A unified system that combines live satellite detection, weather APIs, and machine learning to provide predictive fire risk heatmaps—all in one interactive tool.

🚀 Technologies Used
Component	Technology
Programming Language	Python
Visualization	Folium (Leaflet.js)
Machine Learning	Scikit-learn
Satellite Data	NASA FIRMS
Weather Data	OpenWeatherMap API
Data Handling	Pandas, NumPy
Mapping/Grid Simulation	NDVI Generator

🔄 How It Works
🔧 System Flow
mermaid
Copy
Edit
graph TD
    User -->|Enter Location & API Key| System
    System -->|Fetch Weather + NDVI| Grid
    Grid -->|Predict Risk| MLModel
    MLModel -->|Visualize Map| Folium
    System -->|Save CSV & Map| Output
🧭 Use Case Diagram

🏗️ Architecture Diagram
mathematica
Copy
Edit
┌─────────────────────────────┐
│        User Input           │
│ (Lat, Lon, API Keys, Forest)│
└────────────┬────────────────┘
             ↓
┌─────────────────────────────┐
│  Weather & NDVI Simulator   │
└────────────┬────────────────┘
             ↓
┌─────────────────────────────┐
│     Feature Generator       │
│ (Temp, Humidity, Wind, NDVI)│
└────────────┬────────────────┘
             ↓
┌─────────────────────────────┐
│     ML Fire Risk Model      │
└────────────┬────────────────┘
             ↓
┌─────────────────────────────┐
│     Map + CSV Exporter      │
└─────────────────────────────┘
🛠️ How to Run
Clone this repo:

bash
Copy
Edit
git clone https://github.com/yourusername/fire-risk-map
cd fire-risk-map
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the main script:

bash
Copy
Edit
python forest_fire_risk.py
Enter:

Latitude & Longitude

Your OpenWeatherMap API Key

📁 Output
✅ Interactive fire risk map (fire_risk_map_<timestamp>.html)

✅ CSV report (fire_risk_predictions.csv)

✅ Terminal prints accuracy and summary

📌 Example
📍 Location: Srisailam Forest, India
🌤️ Weather: 32°C, 40% humidity, 10 m/s wind
🔥 High Risk Zones: 62 / 250
📊 Model Accuracy: 96.2%
✅ Map + CSV saved!

📌 Future Enhancements
🛰️ Live satellite NDVI input

⏱️ Time series forecasting

📱 Mobile app integration

🗺️ 3D terrain-aware fire modeling

📩 Auto-alert system for fire-prone zones

🙌 Contributors
👨‍💻 Shaik Sameer – Indian Institute of Technology Patna

Anjali Ray - Indian Institute of Technology Patna

Ritu Rajhans - Indian Institute of Technology Patna

Milan Raj - Chandigarh University

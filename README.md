# 🌱 PlantCare – Intelligent Plant Health Monitoring & Care Advisor Using Fuzzy Logic

**Soft Computing Mini Project**

PlantCare is a web-based intelligent plant care application developed using Python and Mamdani Fuzzy Logic.

It analyses temperature, humidity and optional leaf images to estimate plant stress levels and provide suitable plant care recommendations.

---

## 1. Project Overview

The main purpose of PlantCare is to help users understand plant health conditions through intelligent environmental analysis.

The application considers:
- Plant type
- Plant location
- Temperature
- Humidity
- Leaf photograph (optional)

Based on these inputs, the system calculates plant stress risk and suggests suitable care actions.

## 2. Project Objectives

- To monitor plant environmental conditions.
- To implement Mamdani Fuzzy Logic.
- To estimate plant stress levels.
- To analyse leaf colour using image processing.
- To generate intelligent plant care recommendations.

## 3. Features

1. **Plant Selection:** Supports 71 different plant profiles.
2. **Live Weather:** Fetches outdoor weather information using Open-Meteo.
3. **Manual Readings:** Allows users to enter temperature and humidity manually.
4. **Leaf Image Analysis:** Estimates green, yellow and brown leaf-colour percentages.
5. **Fuzzy Logic Analysis:** Calculates climate stress and overall plant risk.
6. **Membership Functions:** Displays fuzzy membership graphs.
7. **Activated Rules:** Shows the fuzzy rules used in the analysis.
8. **Analysis Graphs:** Displays control surfaces and comparison graphs.
9. **Care Recommendations:** Provides suggestions according to the analysis.

## 4. Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming |
| Flask | Backend development |
| Mamdani Fuzzy Logic | Stress and risk calculation |
| NumPy | Numerical operations |
| Pillow | Image processing |
| Matplotlib | Graphs and visualization |
| HTML | Webpage structure |
| CSS | Website design |
| JavaScript | Frontend interactions |
| Open-Meteo API | Weather information |

## 5. Algorithm Used

**Mamdani Fuzzy Inference System**

PlantCare uses a two-stage fuzzy logic approach.

**Stage 1: Climate Stress Analysis**

Inputs:
- Temperature
- Humidity

Membership categories:
- Temperature: Cold, Ideal, Hot
- Humidity: Dry, Ideal, Humid

Output: Climate Stress Score.

**Stage 2: Overall Plant Risk Analysis**

Inputs:
- Climate Stress
- Leaf Damage

Membership categories:
- Leaf Damage: Healthy, Mild, Severe

Output: Overall Plant Risk Score.

Each stage uses 9 fuzzy rules.

The system uses trapezoidal membership functions, minimum for AND, maximum aggregation and centroid defuzzification.

## 6. Working Process

1. Select a plant type.
2. Select where the plant is kept.
3. Enter the city to fetch weather information.
4. Enter manual temperature and humidity readings if available.
5. Upload a leaf photograph (optional).
6. Click on Analyse My Plant.
7. View the stress score, activated rules and care recommendations.

## 7. Project Visualizations

PlantCare provides:

- Temperature Membership Functions
- Humidity Membership Functions
- Leaf Damage Membership Functions
- Output Membership Functions
- 3D Control Surface
- 2D Climate Stress Map
- Fuzzy vs If-Else Comparison

## 8. Project Structure

```text
PlantCare/
│
├── app.py
├── fuzzy_engine.py
├── crisp.py
├── vision.py
├── plots.py
├── requirements.txt
├── profiles.json
│
├── data/
│   ├── plants.csv
│   └── readings.csv
│
├── templates/
│   └── index.html
│
└── static/
    ├── style.css
    ├── script.js
    └── plots.js
```

## 9. Installation and Execution

**Step 1:** Clone the repository.

```bash
git clone https://github.com/YOUR-USERNAME/PlantCare-Fuzzy-Logic-Advisor.git
```

**Step 2:** Open the project folder.

```bash
cd PlantCare
```

**Step 3:** Create a virtual environment.

```bash
python -m venv venv
```

**Step 4:** Activate the environment (Windows).

```powershell
.\venv\Scripts\Activate.ps1
```

**Step 5:** Install the required libraries.

```bash
pip install -r requirements.txt
```

**Step 6:** Run the project.

```bash
python app.py
```

**Step 7:** Open the application in your browser.

http://127.0.0.1:5000

## 10. Applications

- Home Gardening
- Indoor Plant Monitoring
- Balcony Gardening
- Smart Gardening
- Plant Care Assistance

## 11. Future Scope

- IoT sensor integration.
- Advanced plant disease detection.
- Mobile application development.
- Soil moisture monitoring.
- Historical plant health tracking.
- Support for more plant species.

## 12. Limitations

- Leaf image analysis estimates colour proportions; it does not diagnose diseases.
- Outdoor weather may differ from indoor conditions.
- Plant environmental ranges are approximate.
- Image lighting can affect colour analysis.

## 13. Conclusion

PlantCare demonstrates the practical application of Soft Computing through Mamdani Fuzzy Logic. It combines environmental information and leaf image analysis to estimate plant stress and provide useful care recommendations.

The project makes plant monitoring more intelligent, understandable and user-friendly.

---

**PlantCare – Making Plant Care Smarter with Fuzzy Logic.** 🌱

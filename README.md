# 🇧🇴 Bolivia NDVI Time Series Animation

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Google Earth Engine](https://img.shields.io/badge/Google-Earth%20Engine-4285F4?logo=google)](https://earthengine.google.com/)
[![MODIS](https://img.shields.io/badge/Data-MODIS-2D9B2E)](https://modis.gsfc.nasa.gov/)
[![Python](https://img.shields.io/badge/Python-3.7+-3776AB?logo=python)](https://www.python.org/)

An interactive animation showing **monthly vegetation health (NDVI)** across Bolivia from 2000-2020 using MODIS satellite data.

📊 **Data Source:** NASA MODIS/MOD13A2 (2000-2020)

---

## 🎬 Animation Preview

<div align="center">
  <img src="bolivia_ndvi_clean_fixed.gif" alt="Bolivia NDVI Animation" width="100%" style="max-width: 800px; border-radius: 10px; box-shadow: 0 4px 15px rgba(0,0,0,0.2);">
</div>

*Monthly median NDVI animation showing vegetation changes from January to December across Bolivia*

---

## 🌍 Interactive Web Viewer

<div align="center">
  <iframe src="index.html" width="100%" height="550px" style="border: 2px solid #2D9B2E; border-radius: 10px; box-shadow: 0 4px 15px rgba(0,0,0,0.1);" title="Bolivia NDVI Interactive Viewer"></iframe>
</div>

> 💡 **Tip:** The viewer above is fully interactive! Use the play/pause buttons, keyboard controls (Space, Arrow keys), or click through months manually.

🔗 **[Open Full Interactive Viewer](index.html)** | **[View on GitHub Pages](https://zafariabbas68.github.io/Bolivia-NDVI-Time-Series-Animation)**

---

## 📊 What is NDVI?

**NDVI (Normalized Difference Vegetation Index)** measures vegetation health and density using satellite imagery. It's calculated from red and near-infrared light reflected by plants.

| NDVI Range | Color | Vegetation Status |
|------------|-------|-------------------|
| < 0.1 | 🟤 Dark Brown | Barren land, Altiplano, desert |
| 0.1 - 0.2 | 🟡 Tan | Very sparse vegetation |
| 0.2 - 0.3 | 🟡 Light Gold | Sparse vegetation, dry grasslands |
| 0.3 - 0.4 | 🟢 Yellow-Green | Grasslands, transition zones |
| 0.4 - 0.5 | 🟢 Lime Green | Active croplands, shrubs |
| 0.5 - 0.6 | 🟢 Bright Green | Healthy vegetation |
| 0.6 - 0.7 | 🌲 Forest Green | Forest canopy |
| 0.7 - 0.8 | 🌲 Dark Green | Dense rainforest |
| > 0.8 | 🌲 Deepest Green | Very dense, pristine rainforest |

---

## 🌿 Bolivia's Diverse Ecosystems

Bolivia's unique geography creates dramatic seasonal vegetation patterns across five major eco-regions:

| Region | Location | Characteristics | NDVI Pattern |
|--------|----------|----------------|--------------|
| **Amazon Basin** | North | Dense tropical rainforest, high rainfall | Consistently high NDVI year-round (0.6-0.8) |
| **Yungas** | Central/North | Cloud forests, steep valleys, high biodiversity | Moderate to high, seasonal peaks |
| **Chaco** | Southeast | Dry forests, savannas, thorn scrub | High seasonal variation (0.2 to 0.6) |
| **Altiplano** | West | High-altitude grasslands, arid conditions | Low NDVI (0.1-0.2), subtle changes |
| **Pantanal Lowlands** | East | Seasonal wetlands, flooding patterns | Variable, follows flood cycles |

---

## 🎯 Animation Features

| Feature | Description |
|---------|-------------|
| ✅ **12 monthly frames** | Complete seasonal progression from January to December |
| ✅ **Wet/Dry season indicators** | Green (Nov-Apr) / Orange (May-Oct) visual cues |
| ✅ **Interactive controls** | Play, pause, previous, next, and loop buttons |
| ✅ **Keyboard shortcuts** | Space (play/pause), Arrow keys (navigate months) |
| ✅ **High-quality frames** | 1200px resolution individual images |
| ✅ **Auto-play on load** | Animation starts automatically after 2 seconds |
| ✅ **Mobile-responsive** | Works on desktop, tablet, and mobile devices |

---

## 📈 Seasonal NDVI Patterns in Bolivia

### 🌧️ Wet Season (November - April)

| Month | NDVI Pattern |
|-------|--------------|
| **November** | Green returning to lowlands, Amazon basin vibrant |
| **December** | Rainforest deep green, flooding begins in lowlands |
| **January** | Peak vegetation, Amazon at maximum greenness |
| **February** | Rainforest maximum, Yungas bright green |
| **March** | Peak green season, Chaco region greening |
| **April** | Transition month, green begins to fade in Chaco |

### ☀️ Dry Season (May - October)

| Month | NDVI Pattern |
|-------|--------------|
| **May** | Dry season begins, brown tones appear in Chaco |
| **June** | Altiplano brown, Chaco vegetation minimal |
| **July** | Maximum dry extent across lowlands |
| **August** | Driest month, minimal vegetation in Altiplano |
| **September** | Beginning of transition, vegetation stress visible |
| **October** | Pre-wet season dryness, anticipation of rains |

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| **Google Earth Engine** | Satellite data processing and analysis |
| **MODIS/MOD13A2** | 16-day NDVI composites (1km resolution) |
| **Python** | Data extraction and processing script |
| **PIL/Pillow** | Frame annotation and image processing |
| **JavaScript/HTML/CSS** | Interactive web viewer |
| **ImageMagick** | GIF optimization and compilation |

---

## 📁 Project Structure
Bolivia-NDVI-Time-Series-Animation/
├── index.html # Interactive web viewer
├── bolivia_ndvi_clean_fixed.gif # Main animated GIF
├── annotated_clean/ # Individual monthly frames
│ ├── clean_01.png # January frame
│ ├── clean_02.png # February frame
│ ├── clean_03.png # March frame
│ ├── clean_04.png # April frame
│ ├── clean_05.png # May frame
│ ├── clean_06.png # June frame
│ ├── clean_07.png # July frame
│ ├── clean_08.png # August frame
│ ├── clean_09.png # September frame
│ ├── clean_10.png # October frame
│ ├── clean_11.png # November frame
│ ├── clean_12.png # December frame
└── README.md # Project documentation

text

---

## 🚀 How to Run Locally

### Option 1: Direct Browser (Easiest)

```bash
# Clone the repository
git clone https://github.com/zafariabbas68/Bolivia-NDVI-Time-Series-Animation.git
cd Bolivia-NDVI-Time-Series-Animation

# Open index.html in your browser
open index.html        # On macOS
start index.html       # On Windows
xdg-open index.html    # On Linux
Option 2: Python HTTP Server

bash
# Start a local server
python -m http.server 8000

# Open your browser and go to:
# http://localhost:8000
Option 3: VS Code Live Server

Open project in VS Code
Right-click on index.html
Select "Open with Live Server"
🎮 Interactive Viewer Controls

Control	Action	Keyboard Shortcut
▶ Play	Start auto-playing animation	Space (if paused)
⏸ Pause	Stop animation	Space (if playing)
⏮ Previous	Go back one month	← Left Arrow
⏭ Next	Go forward one month	→ Right Arrow
🔄 Loop	Toggle infinite loop	L key
Additional Controls:

Animation speed: 0.8 seconds per frame
Frame rate: 1.25 FPS (optimized for viewing)
Loop default: On
🎨 Color Legend

Color	Hex Code	NDVI	Interpretation
🟤 Dark Brown	#8B4513	0.0-0.1	Barren land, Altiplano
🟡 Tan	#D2B48C	0.1-0.2	Very sparse vegetation
🟡 Pale Goldenrod	#EEE8AA	0.2-0.3	Sparse vegetation, dry grasslands
🟢 Yellow-Green	#9ACD32	0.3-0.4	Grasslands
🟢 Lime Green	#32CD32	0.4-0.5	Croplands, active vegetation
🟢 Bright Green	#228B22	0.5-0.6	Healthy vegetation
🌲 Forest Green	#006400	0.6-0.7	Forest canopy
🌲 Dark Green	#00441B	0.7-0.8	Dense rainforest
🌲 Deepest Green	#002800	>0.8	Pristine, very dense forest
📊 Key Research Findings

Bolivia's Vegetation Dynamics (2000-2020)

Metric	Value
Maximum NDVI	~0.85 (Amazon Basin, March)
Minimum NDVI	~0.08 (Altiplano, August)
Peak green season	November - April (6 months)
Driest period	May - October (6 months)
Most consistent NDVI	Amazon Basin (year-round >0.6)
Most variable NDVI	Chaco region (0.2 to 0.6)
NDVI range	0.77 (max-min difference)
🔬 Data Processing Methodology

1. Satellite Data Acquisition

Source: NASA MODIS (Moderate Resolution Imaging Spectroradiometer)
Product: MOD13A2 (16-day NDVI composites)
Resolution: 1km per pixel
Time period: 2000-01-01 to 2020-12-31
Total images processed: 478 images
2. Processing Steps

Filter MODIS collection for Bolivia boundary
Create monthly median composites (12 months)
Aggregate 21 years of data per month
Apply NDVI color palette visualization
Generate 12 high-resolution frames (1200px)
Annotate with month labels and season indicators
Compile into animated GIF (2 FPS, 12 frames)
Build interactive HTML/CSS/JS viewer
3. Quality Control

Removed cloudy/poor quality pixels
Applied temporal smoothing
Consistent color scaling across all frames
Validated against ground truth data
🌐 Live Demo

👉 View Live Interactive Map

The live version hosted on GitHub Pages includes:

Auto-playing animation on load
Full interactive controls
Keyboard navigation shortcuts
Season indicators
Mobile-responsive design
No installation required
🗺️ Geographic Coverage

The animation covers the entire territory of Bolivia (1,098,581 km²):

Region	Area (km²)	% of Bolivia	Key Vegetation Features
Amazon Basin	~400,000	36%	Dense rainforest, high NDVI year-round
Andean Region	~300,000	27%	Altiplano, mountains, low NDVI
Chaco Region	~200,000	18%	Dry forests, highly seasonal NDVI
Yungas Valley	~100,000	9%	Cloud forests, transition zone
Pantanal Lowlands	~98,581	10%	Wetlands, flood-dependent NDVI
📸 Monthly Frames Gallery

Month	Season	NDVI Pattern	Key Observation
🇧🇴 January	Wet	Amazon deep green	Peak vegetation, maximum NDVI
🇧🇴 February	Wet	Rainforest maximum	Yungas bright green, flooding
🇧🇴 March	Wet	Peak green season	Amazon most vibrant
🇧🇴 April	Wet	Transition begins	Chaco region greening
🇧🇴 May	Dry	Dry season onset	Brown tones appear
🇧🇴 June	Dry	Altiplano brown	Chaco vegetation minimal
🇧🇴 July	Dry	Maximum dry extent	Lowest NDVI values
🇧🇴 August	Dry	Peak drought	Driest month across Bolivia
🇧🇴 September	Dry	Transition	Early green return in lowlands
🇧🇴 October	Dry	Pre-wet season	Most extreme dryness
🇧🇴 November	Wet	Green returning	Amazon rejuvenation begins
🇧🇴 December	Wet	Rainforest recovery	Full green across basin
🤝 Contributing

Contributions are welcome! Here's how to help improve this project:

Ways to Contribute

Code improvements
Documentation updates
Bug reports
Feature requests
Data analysis enhancements
How to Submit Changes

Fork the repository
Create a feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add some amazing feature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request
Planned Improvements

Add time series comparison with 2020-2024 data
Include rainfall data overlay
Add regional GDP/agricultural correlation
Implement month slider for custom playback speed
Add download option for individual frames
Create side-by-side comparison with historical averages
📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments

NASA - MODIS satellite data and science team
Google Earth Engine - Free processing platform
USGS - Boundary data (USDOS/LSIB_SIMPLE)
Hakai Institute - Color palette inspiration
OpenStreetMap - Geographic reference data
📧 Contact

Developer: Abbas Zafari

GitHub: @zafariabbas68
Project Repository: https://github.com/zafariabbas68/Bolivia-NDVI-Time-Series-Animation
Live Demo: https://zafariabbas68.github.io/Bolivia-NDVI-Time-Series-Animation
📚 Citation

If you use this animation in research or publications, please cite:

bibtex
@misc{zafari2024bolivia,
  author = {Zafari, Abbas},
  title = {Bolivia NDVI Time Series Animation 2000-2020},
  year = {2024},
  publisher = {GitHub},
  url = {https://github.com/zafariabbas68/Bolivia-NDVI-Time-Series-Animation}
}
⭐ Show Your Support

If you find this project useful for:

🌍 Climate change research
🌾 Agricultural monitoring
🌳 Deforestation studies
🎓 Educational purposes
📊 Data visualization inspiration
Please ⭐ star this repository!

Your support helps make this project better and reach more people.

Built with Google Earth Engine, Python, and ❤️ for Bolivia's natural heritage

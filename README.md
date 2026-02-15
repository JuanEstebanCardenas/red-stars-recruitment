# ⚽ 2026 Recruitment Strategy: Forward Succession Plan
### Project Lead: Juan Cardenas Urrego

## 📌 Project Overview
This repository contains a data-driven scouting model designed to identify a tactical successor for **Ludmila** (Chicago Red Stars) using performance data from the **Frauen-Bundesliga**. 

The goal was to find a "Speed Merchant" profile that matches Ludmila’s high-volume ball progression while identifying players with a higher probability of converting chances into goals (npxG).

## 📂 Repository Structure
- `scouting_mode_similarity.ipynb`: The primary model using **Cosine Similarity** and **Min-Max Scaling** to rank players based on tactical fit.
- `scouting_model_2nd.ipynb`: Risk mitigation analysis, including the "League Tax" adjustment for players transitioning from Germany to the NWSL.
- `2026 Recruitment Strategy - Forward Succession Plan.pdf`: The final executive presentation delivered to the Technical Director.
- `data/`: Contains the raw performance datasets for the NWSL and Bundesliga.

## 🛠️ Technical Stack
- **Python**: Core analysis.
- **Pandas & NumPy**: Data cleaning (handling international character encoding and string-to-float conversions for minutes played).
- **Scikit-Learn**: Implemented `MinMaxScaler` for normalization and `cosine_similarity` for player profiling.
- **Matplotlib & Seaborn**: Statistical heatmaps and performance distributions.
- **MPLSoccer**: Visualizing player traits via Pizza Plots.

## 📊 Key Insights
- **Primary Target:** Identified **Jule Brand** (VfL Wolfsburg) as the 99.1% similarity match to Ludmila.
- **The "Germany Advantage":** Quantitative analysis proved that Bundesliga prospects are **22.2% more likely** to become elite NWSL starters compared to domestic draft picks.
- **Risk Mitigation:** Applied a conservative "League Effect" correction factor to discount European stats, ensuring the projections remain realistic for the physical jump to the NWSL.

## 🚀 How to Run
1. Clone the repository.
2. Ensure you have the virtual environment set up:
   ```bash
   pip install -r requirements.txt
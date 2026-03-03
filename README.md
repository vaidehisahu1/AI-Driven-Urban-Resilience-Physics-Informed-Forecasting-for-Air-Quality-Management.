# AI-Driven-Urban-Resilience-Physics-Informed-Forecasting-for-Air-Quality-Management.

🌍 Overview
This project proposes a Decision Support System (DSS) that utilizes Physics-Informed Artificial Intelligence to create a dynamic "Digital Twin" of a city’s air quality. Unlike standard "black box" models, our architecture integrates atmospheric physics—specifically wind dispersion dynamics—directly into the neural network.

The system is designed to transition urban planning from Reactive (Static Bans) to Proactive (Dynamic Zoning). It forecasts pollution levels 24 hours in advance and simulates "What-If" policy scenarios (e.g., traffic reduction impact), enabling targeted interventions in specific micro-clusters.

🎯 Problem Statement
Current pollution control measures (like the Graded Response Action Plan - GRAP) are reactive, implemented only after air quality crosses "Severe" thresholds. This leads to:

Economic Disruption: Blanket construction bans hurt livelihoods.
Public Health Risks: Delayed response to toxic spikes.
Inefficient Planning: Lack of granular data to identify "Stagnation Zones" vs. "Traffic Hotspots."
💡 The Solution
We developed a Physics-Informed LSTM (Long Short-Term Memory) model that predicts PM2.5 levels based on meteorological and pollution data. Our key innovation is a custom Physics Loss Function that penalizes the model if it predicts scenarios that violate the laws of wind dispersion.

Key Features:

High Accuracy Forecasting: Predicting PM2.5 with high reliability.
Scenario Simulation: Quantifying the impact of policy changes (e.g., "A 20% traffic reduction yields a 17% drop in pollution").
Urban Stress Index: Clustering city zones to guide specific infrastructure investments (Green buffers vs. EV stations).
📊 Results
Our prototype, trained on Delhi pollution data (CPCB & Satellite sources), achieved:

RMSE: 12.29 µg/m³ (High Precision).
Policy Simulation: Validated that targeted traffic reduction creates significant air quality improvements.
Zoning: Successfully identified distinct "Urban Metabolism" archetypes for Delhi.
📁 Repository Contents
This repository contains all necessary files to understand and reproduce our work.

FILE / FOLDER
DESCRIPTION
Project_Presentation.pptx	The slide deck detailing the problem, solution, and urban planning impact.
Project_Video.mp4	A video walkthrough of the project idea and technical implementation.
Urban_Metabolism_Model.ipynb	The Python notebook containing data preprocessing, model architecture, and training loops.
README.md	This file.

🛠️ Tech Stack & Dependencies
Language: Python 3.x
Deep Learning: PyTorch (LSTM Architecture)
Data Processing: Pandas, NumPy
Machine Learning: Scikit-Learn (Clustering, Scaling)
Visualization: Matplotlib, Seaborn

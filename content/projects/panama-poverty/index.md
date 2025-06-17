+++
title = "Poverty Classification with Multi-Modal Data"
date = 2025-05-01
summary = "Using satellite and minimal survey data to predict household poverty in Panama."
+++

**What it does**  
This project develops a hybrid machine learning framework to improve household-level poverty classification by integrating satellite-derived features and a minimal set of survey-based proxy means test (PMT) questions.

[![Demo GIF](/images/projects/200OK_gif.gif)](https://youtu.be/vDS_DnzB0eU?si=zDLkQgEyNNFDXd3b)



**Why I made it**  
My motivation was grounded in the needs of governments and non-profit organizations that must target benneficiaries under tight budget constraints. Comprehensive living standards surveys are axpensive and slow, while purely geospatial methods lack granularity. By merging both approaches, this model enables two use cases: 
1. organizations with no field resources can generate reliable poverty estimates from geolocation alone;
2. organizations with limited resources can improve targeting accuracy using 5 simple survey questions.

**Tools & Technologies**  
- Feature extraction: MOSAIKS API, VIIRS API
- Database storage: Parquet, ChromaDB
- Geospatial analysis: shapely, geopandas
- Machine Learning: sklearn, interpretml
- Data Visualization: folium, matplotlib
- App Development: html, flask, webbrowser, threading


**What I learned**  
- Working with high-resolution VIIRS data and MOSAIKS features.
- Deploying interpretable ML.  
- Building full pipelines from model training to deployment.
- Creating interactive apps with an html front-end and hosted using flask.

**Real-world use / impact**  
Used to demonstrate a low-cost poverty targeting prototype during a university presentation on data-driven development. The approach has potential to support NGOs and governments in allocating social resources more efficiently, especially in data-scarce settings.

**Team**  
Built alongside Ángela López and César Nuñez as a final project of the CAPP30254 Machine Learning for Public Policy class.

🔗 **Code**  
[View on GitHub](https://github.com/manucardona/)
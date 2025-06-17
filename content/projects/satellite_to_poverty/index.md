+++
title = "Poverty rate prediction using multi-modal survey and earth observation data"
date = 2023-07-21
summary = "Using satellite and minimal survey data to predict regional poverty rates in Ethiopia."
+++

**What it does**  
This project uses a multi-modal machine learning pipeline that:

1. Extractes visual features from freely available Sentinel-2 satellite imagery (10m resolution) using the MOSAIKS API.
2. Combines these features with survey data from Ethiopia's nationally representative LSMS dataset.
3. Trains several classification models to predict household-level poverty status.
4. Estimates regional poverty rates as a weighted average of predictions.
5. Optimizes survey design by selecting questions that are most complementary to image-based features.

This approach improves prediction while minimizing data collection burdens.

![Demo Image](/images/projects/satelite_roc.jpeg)



**Why I made it**  
Traditional poverty measurement relies on long and costly household surveys, which are often infeasible for frequent or large-scale data collection. This project seeks to bridge the gap by integrating satellite imagery with a minimal set of survey questions to create a reliable, low-cost poverty estimation tool. This hybrid approach is particularly useful for:

- Governments or NGOs needing poverty data where survey infrastructure is weak.
- Programs operating under severe cost or time constraints that still require household-level poverty targeting.

**Tools & Technologies**  
- **Tools**: Python, scikit-learn, LightGBM, MOSAIKS, PCA, Sentinel-2 imagery (via Microsoft Planetary Computer)
- **Techniques**: Proxy Means Tests, feature selection, image featurization, supervised classification, bootstrapping, error decomposition


**What I learned**  
Key takeaways include:

- Process and integrate satellite imagery using Sentinel-2 data and the Microsoft Planetary Computer, including selecting cloud-free tiles and aligning imagery to survey clusters.
- Engineer survey data for predictive modeling, including transforming categorical responses, handling missing values, and converting full surveys into interpretable binary variables.
- Train and evaluate supervised models (e.g., LightGBM, EBMs) for binary classification tasks, incorporating sample weights and stratified train-test splits to match national poverty distributions.
- Design and evaluate proxy means tests (PMTs) by selecting optimal subsets of survey questions and combining them with geospatial features.
- Measure model performance using custom metrics, such as poverty rate error (PRE), and perform rigorous evaluation using cross-validation and bootstrapped confidence intervals.
- Balance model simplicity and interpretability for use cases involving policymakers, demonstrating that lightweight models can outperform black-box approaches when designed well.


**Real-world use / impact**  
This work demonstrates that satellite image features can:
- Replace or complement survey data when unavailable.
- Support better targeting of poverty interventions.
- Enable cost-effective, scalable poverty monitoring in developing regions.

It also contributes methodological advances by proposing:
- A survey + image guided variable selection method, which selects survey questions that are maximally informative when combined with remote sensing data.
- A non-deep-learning-based image featurization pipeline that is both interpretable and computationally lightweight.


**Team**  
- Simone Fobi (Microsoft AI for Good Lab)  
- Manuel Cardona (IPA)  
- Elliott Collins (IPA)  
- Caleb Robinson, Anthony Ortiz, Tina Sederholm, Rahul Dodhia, Juan Lavista Ferres (Microsoft AI for Good Lab)

🔗 **Code**  
[View on GitHub](https://github.com/manucardona/satellite_to_poverty/tree/master)
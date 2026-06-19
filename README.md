# Space X Analysis 🚀
### SpaceX Falcon 9 First Stage Landing Prediction Capstone Project

---

## 📌 Project Overview
The commercial space industry is evolving rapidly, driven heavily by SpaceX's dramatic cost reductions. A single Falcon 9 launch costs approximately **$62 million**, whereas competing rocket providers often charge upwards of **$165 million**. This massive cost edge is primarily achieved by **reusing the first stage booster**. 

This repository contains the complete capstone project codebase aimed at predicting whether the first stage of a Falcon 9 rocket will land successfully. By applying Data Science techniques and Machine Learning algorithms, this project enables competitive analysis, cost forecasting, and operational predictability for future space launches.

---

## 🛠️ Project Workflow & Methodology

The project follows a comprehensive end-to-end data science lifecycle:

1. **Data Collection (API & Scraping):**
   * Retrieved unstructured launch parameters from the **SpaceX REST API**.
   * Extracted historical tabular data from Wikipedia pages via web scraping with **BeautifulSoup**.
2. **Data Wrangling:**
   * Filtered relevant parameters, managed missing values, and engineered data profiles.
   * Converted raw landing cases into binary labels (`1` for successful landing, `0` for unsuccessful/no attempt).
3. **Exploratory Data Analysis (EDA):**
   * Performed targeted data exploration using **SQL queries (SQLite)** to aggregate records, calculate operational statistics (e.g., payload mass averages), and track optimal booster versions.
   * Visualized parameter relationships (Flight Number, Launch Sites, Payload Mass, Orbit types) using `matplotlib` and `seaborn`.
4. **Interactive Visual Analytics:**
   * **Folium Map Application:** Charted launch configurations, established marker clusters for success/failure rates, and drew explicit polyline metrics to measure physical proximity to coastlines, railways, highways, and municipal infrastructure.
   * **Plotly Dash Dashboard:** Built a responsive, real-time analytics panel featuring dropdown components and continuous payload mass sliders to filter core distributions instantly.
5. **Predictive Machine Learning Classification:**
   * Scaled feature metrics utilizing `StandardScaler` and partitioned historical data arrays into training and testing sets.
   * Formulated optimized hyperparameters using `GridSearchCV` across multiple classification paradigms.

---

## 📊 Key Insights & Results

* **Launch Site Performance:** Geospatial mapping indicated that **CCAFS LC-40** drove the highest volume of launch logs, whereas **KSC LC-39A** displayed a specific launch success rate of **76.9%**.
* **Temporal Trend:** Annual trends from 2010 to 2020 demonstrated a steady upward trajectory in first-stage recovery optimization over time.
* **Orbit Analysis:** High-altitude orbits (such as ES-L1, GEO, HEO, and SSO) yielded a perfect 100% recovery factor within the scope of this baseline data block.
* **Model Evaluation:** The hyperparameter-tuned **Decision Tree Classifier** and **Random Forest Classifier** delivered peak accuracy metrics, establishing an **83% test accuracy** score with low false-negative outcomes in the finalized confusion matrix.

---

## 📂 Repository Structure & Project Labs

Navigate below to access specific interactive notebooks and source codes detailing each milestone phase:

* 🔌 **Data Collection (API):** [jupyter-labs-spacex-data-collection-api.ipynb](https://github.com/Dineth-Wickremasinghe/SpaceX-Analysis/blob/main/Notebooks/jupyter-labs-spacex-data-collection-api.ipynb)
* 🌐 **Data Collection (Scraping):** [jupyter-labs-webscraping.ipynb](https://github.com/Dineth-Wickremasinghe/SpaceX-Analysis/blob/main/Notebooks/jupyter-labs-webscraping.ipynb)
* 🧼 **Data Wrangling:** [labs-jupyter-spacex-Data wrangling.ipynb](https://github.com/Dineth-Wickremasinghe/SpaceX-Analysis/blob/main/Notebooks/labs-jupyter-spacex-Data%20wrangling.ipynb)
* 📉 **EDA with Data Visualization:** [edadataviz.ipynb](https://github.com/Dineth-Wickremasinghe/SpaceX-Analysis/blob/main/Notebooks/edadataviz.ipynb)
* 🗄️ **EDA with SQL Queries:** [jupyter labs eda sql coursera sqllite.ipynb](https://github.com/Dineth-Wickremasinghe/SpaceX-Analysis/blob/main/Notebooks/jupyter%20labs%20eda%20sql%20coursera%20sqllite.ipynb)
* 🗺️ **Geospatial Maps (Folium):** [lab jupyter launch site location.ipynb](https://github.com/Dineth-Wickremasinghe/SpaceX-Analysis/blob/main/Notebooks/lab%20jupyter%20launch%20site%20location.ipynb)
* 📊 **Interactive Dash Dashboard:** [spacex-dash-app.py](https://github.com/Dineth-Wickremasinghe/SpaceX-Analysis/blob/main/Notebooks/spacex-dash-app.py)
* 🤖 **Predictive Classification (ML):** [SpaceX Machine Learning Prediction Part 5.ipynb](https://github.com/Dineth-Wickremasinghe/SpaceX-Analysis/blob/main/Notebooks/SpaceX%20Machine%20Learning%20Prediction%20Part%205.ipynb)

---

## 🏁 Conclusion
By analyzing the technical and financial constraints of Falcon 9 components, this project establishes a reliable template for optimizing commercial space configurations. Predicting the physical recoverability of rocket boosters enables smarter operational roadmaps and democratization within space technology sectors.

---

## 👤 Author
* **Dineth Wickremasinghe**
* **Date:** May 25, 2026
* **Affiliation:** IBM Developer Skills Network / Coursera Data Science Capstone Project

---

# 🔋 Energy Consumption Pattern Clustering

## 📌 Project Overview

This project focuses on discovering **common daily energy usage patterns** from **half-hourly energy meter readings** using **unsupervised machine learning**.
By clustering daily load profiles, the analysis reveals interpretable consumption behaviors that can support **energy optimization, demand forecasting, and operational planning**.

---

## 🎯 Objective

* Convert raw half-hourly energy data into **daily load profiles**
* Identify **4–6 distinct usage patterns** using **K-Means clustering**
* Visualize cluster centroids to interpret real-world energy behavior
* Deliver reproducible and shareable results

---

## 🛠️ Technologies Used

* **Python**
* **pandas** – data preprocessing & aggregation
* **scikit-learn** – normalization & clustering
* **matplotlib** – visualization

---

## 📂 Dataset

* CSV file containing half-hourly energy/power readings
* Key column:

  * `dt` → timestamp of energy reading
* Frequency: **30 minutes**

---

## 🔄 Methodology

### 1️⃣ Data Loading & Preprocessing

* Load CSV data
* Convert timestamp column (`dt`) to datetime format
* Extract date and half-hour time slots

### 2️⃣ Daily Load Profile Creation

* Aggregate readings into **48 half-hour slots per day**
* Each row represents one day’s energy consumption pattern

### 3️⃣ Normalization

* Apply **StandardScaler**
* Ensures clustering is based on **usage shape**, not absolute consumption

### 4️⃣ Clustering

* Apply **K-Means clustering**
* Use **5 clusters** (within the required 4–6 range)
* Assign each day to a usage pattern

### 5️⃣ Visualization

* Plot cluster centroids as line charts
* Each centroid represents a typical daily energy behavior

---

## 📊 Results & Insights

* Identified multiple distinct daily energy usage patterns
* Cluster centroids reveal behaviors such as:

  * Daytime-heavy office usage
  * Morning-evening residential peaks
  * Consistent high-load industrial patterns
* Results are interpretable and actionable

---

## 📦 Deliverables

* ✅ Jupyter Notebook with full analysis
* ✅ PNG image of cluster centroids
* ✅ CSV files with cluster labels and daily profiles
* ✅ ZIP file containing all outputs

---

## 📁 Repository Structure

```
📦 Energy-Consumption-Pattern-Clustering
 ┣ 📜 energy-consumptions-pattern.ipynb
 ┣ 📊 cluster_centroids.png
 ┣ 📄 daily_energy_clusters.csv
 ┣ 📄 cluster_labels.csv
 ┣ 📦 energy_consumption_clustering_deliverables.zip
 ┗ 📘 README.md
```

---

## ▶️ How to Run

1. Clone the repository
2. Install dependencies:

   ```bash
   pip install pandas scikit-learn matplotlib
   ```
3. Open and run the notebook:

   ```bash
   jupyter notebook energy-consumptions-pattern.ipynb
   ```

---

## 🚀 Future Improvements

* Add elbow and silhouette analysis
* Separate weekday vs weekend patterns
* Apply advanced time-series clustering (e.g., DTW)
* Include anomaly detection for unusual consumption days

---

## 📌 Key Takeaway

This project demonstrates an **end-to-end data science workflow**—from raw time-series data to interpretable insights—using scalable and industry-standard techniques.

---

## 👤 Author

**Swapnanil Chatterjee**

---

If you want, I can next:

* 🔥 Optimize this README for **ATS keywords**
* 🧠 Add a **“Business Impact” section**
* 🎯 Write a **GitHub repo description + tags**
* 📄 Align this README with your **resume bullets**

Just say the word 🚀

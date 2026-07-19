# 🚀 SmartSegment - AI/ML Customer Segmentation

# Mall Customer Segmentation
###  — Hackathon Winning Project(1st place)

A full end-to-end ML pipeline + interactive web dashboard for
**E-Commerce Behavioural Customer Segmentation** using the Mall Customers dataset.

---
RUN WEBSITE HERE!!!
https://smartsegmentbykolarkoders.onrender.com

## 📌 Overview

SmartSegment is an AI-powered customer segmentation project that uses Machine Learning to group customers based on their purchasing behavior and demographic characteristics. By identifying meaningful customer segments, businesses can design personalized marketing campaigns, improve customer engagement, and make data-driven decisions.

---

## 🎯 Problem Statement

Traditional marketing strategies often treat all customers the same, resulting in lower engagement and reduced conversion rates.

This project addresses the problem by applying Machine Learning clustering techniques to identify groups of customers with similar characteristics, enabling targeted and effective marketing.

---

## 💡 Solution

SmartSegment analyzes customer data and automatically groups customers into meaningful segments using clustering algorithms. These segments help businesses understand customer behavior and optimize marketing strategies.

---

## ✨ Features

* 📊 Customer Data Analysis
* 🧹 Data Cleaning & Preprocessing
* 📈 Exploratory Data Analysis (EDA)
* 🤖 Machine Learning-Based Customer Segmentation
* 📉 Cluster Visualization
* 📋 Business Insights & Recommendations
* ⚡ Fast and Easy to Use

---

## 🛠️ Technology Stack

*Programming Languages

Python

*Machine Learning

Scikit-learn
K-Means Clustering
StandardScaler
Silhouette Analysis
Elbow Method
Joblib

*Data Processing

Pandas
NumPy

*Backend

Flask

*Frontend

HTML5
CSS3
JavaScript
Bootstrap

*Visualization

Chart.js
Matplotlib

*Deployment

Railway
Render

---

## 📂 Project Structure


```
mall_segmentation/
│
├── data/
│   ├── Mall_Customers.csv      ← Original dataset (200 customers)
│   └── segmented.csv           ← Generated after training (with Segment column)
│
├── models/
│   ├── kmeans_model.pkl        ← Trained K-Means model (k=5)
│   ├── scaler.pkl              ← Fitted StandardScaler
│   ├── segment_map.pkl         ← Cluster number → segment name mapping
│   └── cluster_stats.pkl       ← Per-cluster summary statistics
│
├── static/
│   ├── scatter.png             ← K-Means scatter plot (generated)
│   ├── elbow_curve.png         ← Elbow + silhouette chart (generated)
│   ├── bar_charts.png          ← 4-panel bar chart (generated)
│   └── gender_pie.png          ← Gender distribution pies (generated)
│
├── templates/
│   ├── base.html               ← Shared nav + layout
│   ├── index.html              ← Main dashboard (metrics + charts)
│   ├── customers.html          ← Customer table with filter
│   ├── segments.html           ← Segment profiles + strategies
│   └── predict.html            ← Live prediction form
│
├── train.py                    ← ML training pipeline
├── app.py                      ← Flask web dashboard
├── requirements.txt            ← Python dependencies
├── run.sh                      ← One-click setup + launch
└── README.md                   ← This file
```

---

## Web Dashboard Pages

| URL | Page | What it shows |
|-----|------|---------------|
| `/` | Dashboard | Metrics, scatter plot, donut, bar charts, summary table |
| `/customers` | Customers | All 200 customers — filterable by segment |
| `/segments` | Segments | Full profile cards with strategies per segment |
| `/predict` | Predict | Live form — input a new customer, get predicted segment |
| `/api/scatter` | JSON API | All customer data for JS scatter chart |
| `/api/stats` | JSON API | Summary statistics |

---

## The 5 Customer Segments

| Segment | Income | Score | Count | Strategy |
|---------|--------|-------|-------|----------|
| Premium VIPs | High ($87k) | High (82) | 39 | Loyalty rewards, VIP events |
| Cautious Wealthy | High ($88k) | Low (17) | 35 | Premium curated offers |
| Standard Shoppers | Mid ($55k) | Mid (50) | 81 | Loyalty programs, cross-sell |
| Impulsive Spenders | Low ($26k) | High (79) | 22 | Flash sales, FOMO campaigns |
| Budget Conscious | Low ($26k) | Low (21) | 23 | Discount bundles, clearance |

---

## ML Pipeline (train.py)

1. Load `Mall_Customers.csv`
2. Feature engineering — Income + Spending Score
3. StandardScaler normalisation
4. Elbow curve + silhouette analysis (k=2 to 10)
5. Final K-Means with k=5
6. Segment naming from centroid coordinates
7. Generate charts (scatter, elbow, bars, gender pies)
8. Save model artifacts with joblib

---

## Tech Stack

- **Python 3.8+**
- **scikit-learn** — K-Means, StandardScaler, silhouette_score
- **pandas / numpy** — Data processing
- **matplotlib / seaborn** — Chart generation
- **Flask** — Web dashboard
- **Chart.js** (CDN) — Interactive browser charts
- **joblib** — Model serialisation

## 📊 Results

The project successfully identifies multiple customer segments based on behavioral and demographic features.

These segments can be used for:

* Personalized Marketing
* Customer Retention
* Product Recommendations
* Business Intelligence
* Sales Strategy Optimization

---

## 📸 Screenshots

### Dashboard

<img width="959" height="535" alt="dashboard" src="https://github.com/user-attachments/assets/a3c12d4d-e84d-4a6a-873b-f074ffb7a02e" />



```
<img width="959" height="535" alt="dashboard" src="https://github.com/user-attachments/assets/fef8ceb8-9926-4d20-b903-9856caf94ee8" />


```

### Customer Clusters

<img width="959" height="500" alt="customer segment" src="https://github.com/user-attachments/assets/63c00b15-5f9d-455b-a5c7-0fb5868b69e9" />


```
<img width="959" height="500" alt="customer segment" src="https://github.com/user-attachments/assets/6e353299-ce44-4d36-918b-376d96a6e922" />

```

### Model Accuracy & Efficiency

<img width="959" height="535" alt="model" src="https://github.com/user-attachments/assets/a45a7d10-92f9-4e75-8d11-567d3b3c6cf8" />


```
<img width="959" height="535" alt="model" src="https://github.com/user-attachments/assets/f1acb74e-22bf-472a-af23-1c0f8444be56" />

```

---
### RFM Metrics - Behavioural Customer Segmentation

<img width="959" height="436" alt="RFM" src="https://github.com/user-attachments/assets/99ac4aac-5991-4d61-b13c-068963b9edb2" />


```
<img width="959" height="436" alt="RFM" src="https://github.com/user-attachments/assets/776c5764-c840-4180-8484-ffe3de798f8f" />

```

---
### Expected Business Impact

<img width="959" height="529" alt="Expected Business Impact" src="https://github.com/user-attachments/assets/3a7aede8-63a3-4f7f-8f82-7828c6ac18da" />


```
<img width="959" height="529" alt="Expected Business Impact" src="https://github.com/user-attachments/assets/5a757504-8b3f-410b-9c6e-5b7386316b34" />

```

---
## 🔮 Future Enhancements

* Deep Learning-based segmentation
* Real-time customer prediction
* Streamlit Web Application
* Flask API Integration
* Interactive Dashboard
* Customer Recommendation System
* Cloud Deployment
* Automated Report Generation

---

## 📚 Skills Demonstrated

* Machine Learning
* Data Analysis
* Customer Analytics
* Data Visualization
* Python Programming
* Business Intelligence
* Clustering Algorithms
* Artificial Intelligence

---

## 🤝 Contributing

Contributions are welcome!

Feel free to fork the repository, create a feature branch, and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Sridharan P**

AI & Machine Learning Student

GitHub: https://github.com/Sridharan03

LinkedIn: https://www.linkedin.com/in/sridharan2028/

---

⭐ If you found this project useful, consider giving it a star!


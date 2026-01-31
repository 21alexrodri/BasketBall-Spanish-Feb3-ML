# 🏀 Basketball Player Clustering (K-Means)

This project applies **unsupervised machine learning (K-Means clustering)** to analyze basketball player statistics and identify **different player profiles** based on their style of play.

All the analysis is contained in a **single Jupyter Notebook**, where the complete process is developed step by step.

🌍 Read this in:
- [English](README.md)
- [Español](README.es.md)
- [Català](README.cat.md)

---

## 📌 Project Description

Using real match statistics from the Spanish Basketball Federation (FEB), this project aims to:

- analyze player performance data  
- extract meaningful basketball features  
- group players with similar playing styles  
- interpret each group from a basketball perspective  

The objective is not prediction, but **understanding player roles through data**.

---

## 🧠 Identified Player Profiles

The clustering process identifies **four main player profiles**:

| Cluster | Description |
|-------|-------------|
| 0 | Offensive wings / scorers |
| 1 | Low-usage rotation players |
| 2 | Playmakers / guards |
| 3 | Dominant interior players |

Each cluster is interpreted using statistical averages and real player examples.

---

## 📊 Features Used

The final clustering model uses the following variables:

- Points per game (`pts`)
- Total rebounds (`trb`)
- Turnovers (`tov`)
- 2-point usage (`usage_2p`)
- 3-point usage (`usage_3p`)
- Paint shot attempts (`paint_shots`)
- Outside shot attempts (`outside_shots`)
- Assist-to-turnover ratio (`ast_tov_ratio`)
- Defensive impact (`defensive_impact`)

All features are standardized before applying K-Means.

---

## 📈 Methodology

The notebook follows these main steps:

1. Data extraction from MongoDB  
2. Data cleaning and preprocessing  
3. Feature engineering  
4. Exploratory data analysis  
5. Feature selection  
6. Data scaling  
7. K-Means clustering  
8. Selection of optimal number of clusters (Elbow & Silhouette methods)  
9. Cluster interpretation  
10. Visualization using PCA  

---

## ⚙️ Technologies Used

- Python  
- Pandas
- Scikit-learn  
- Matplotlib  
- Seaborn  
- MongoDB  
- Jupyter Notebook  

---



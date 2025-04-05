# 🌍 World Happiness Report Clustering Analysis

## 🚀 Project Overview
This project analyzes the World Happiness Report dataset using **K-Means** and **DBSCAN** clustering algorithms to group countries based on socio-economic indicators. The goal is to uncover patterns in happiness metrics and compare the effectiveness of centroid-based vs density-based clustering approaches.

**✨ Key Features**:
- 🧹 Data preprocessing & standardization
- 📊 Optimal cluster determination with Elbow Method
- 🎯 K-Means clustering implementation
- 🌐 DBSCAN clustering with parameter tuning
- 📊 3D visualization of clusters using PCA
- 🔍 Cluster interpretation and algorithm comparison
- 🏆 Bonus: Happiness Score prediction using cluster labels

---

## 📂 Dataset
**World Happiness Report**  
Download the latest dataset from [Kaggle](https://www.kaggle.com/unsdsn/world-happiness) or [World Happiness Report](https://worldhappiness.report/).  
Place the CSV file in the `data/` directory.

**📈 Features Used**:
- 💰 GDP per capita
- 🤝 Social support
- 🩺 Healthy life expectancy
- 🗽 Freedom to make life choices
- 🎁 Generosity
- 🕵️ Perception of corruption

---

## ⚙️ Requirements
- Python 3.8+ <img src="https://img.icons8.com/color/48/000000/python.png" width="20"/>
- pandas <img src="https://img.icons8.com/color/48/000000/pandas.png" width="20"/>
- numpy <img src="https://img.icons8.com/color/48/000000/numpy.png" width="20"/>
- scikit-learn <img src="https://img.icons8.com/color/48/000000/scikit-learn.png" width="20"/>
- matplotlib <img src="https://img.icons8.com/color/48/000000/matplotlib.png" width="20"/>
- seaborn <img src="https://seaborn.pydata.org/_static/logo-wide-lightbg.svg" width="20"/>
- plotly <img src="https://img.icons8.com/color/48/000000/plotly.png" width="20"/>
- jupyter <img src="https://img.icons8.com/color/48/000000/jupyter.png" width="20"/>

---

## 🔬 Methodology
### 1. 🧼 Data Preprocessing
- 🚫 Handle missing values
- 📏 Standardize features using `StandardScaler`
- 🔄 Dimensionality reduction with PCA

### 2. 🧲 K-Means Clustering
- 📐 Determine optimal clusters using Elbow Method
- 🤖 Implement K-Means with `sklearn.cluster.KMeans`
- 📊 Visualize clusters in 2D/3D space

### 3. 🌌 DBSCAN Clustering
- 📈 Find optimal ε using k-distance graphs
- 🎚️ Tune `min_samples` parameter
- 🛠️ Implement DBSCAN with `sklearn.cluster.DBSCAN`
- ↔️ Compare results with K-Means

### 4. 🔍 Advanced Analysis
- 🔎 Interpret cluster characteristics
- 🎯 Identify outlier countries
- ⚖️ Compare algorithm performance
- 🔮 Predict Happiness Score (Bonus Task)

---

## 🆚 Algorithm Comparison
| Metric          | K-Means                     | DBSCAN                      |
|-----------------|-----------------------------|-----------------------------|
| **🔵 Cluster Shapes**  | Spherical                   | Arbitrary                   |
| **🔇 Noise Handling**  | No                          | Yes                         |
| **🎯 Optimal k**       | 4 (Elbow Method)            | Auto-detected               |
| **💡 Key Insights**    | Wealth-health correlation   | Regional density patterns   |

---

## 🏆 Findings
- **Cluster 1** (💰 High GDP/🩺 Life Expectancy): Nordic countries 🇳🇴🇸🇪🇫🇮
- **Cluster 2** (🕵️ Low Corruption/🗽 High Freedom): Western democracies 🇺🇸🇨🇦🇩🇪
- **DBSCAN** identified 3 dense regions + 12% noise 🎭
- **K-Means** clusters align better with regional groupings 🌍

---

## 🌟 Bonus Task
- Used cluster labels as feature in Random Forest regression 🌳
- Achieved **R² score: 0.82** 📈
- **MAE: 0.38** on Happiness Score prediction 🎯

---

## 📜 License
[MIT License](LICENSE) <img src="https://img.icons8.com/color/48/000000/license.png" width="20"/>

---

## 👥 Contributors
- Laiqa Ali <img src="https://img.icons8.com/color/48/000000/user.png" width="20"/>

---

*Made with ❤️ using [Icons8](https://icons8.com) and GitHub Markdown*

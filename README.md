# Anomaly Detection on Social Networks

## 📌 Overview
Anomaly detection in social networks is crucial for identifying fraudulent activities, cyber threats, and unusual user behaviors. This project explores feature-driven anomaly detection and clustering-based techniques to analyze user interactions and detect anomalies in social network graphs. 

We leverage various machine learning techniques to uncover hidden patterns, visualize relationships, and enhance network security by flagging suspicious nodes.

## 📂 Repository Structure

### 📁 `Adetection.ipynb`
- **Purpose:** Implements feature-based anomaly detection using extracted network attributes.
- **Key Steps:**
  - Loads social network data from `.feat` and `.featnames` files.
  - Constructs a feature matrix for network nodes.
  - Applies anomaly detection algorithms (e.g., Isolation Forest, Local Outlier Factor, Autoencoders) to detect deviations.
  - Generates `anomaly_features.csv`, which contains identified anomalies and extracted features.
  - Evaluates model performance and visualizes detected anomalies.

### 📁 `Aclusterning.ipynb`
- **Purpose:** Implements clustering-based anomaly detection using the generated anomaly dataset.
- **Key Steps:**
  - Loads the dataset (`anomaly_features.csv`) created from `Adetection.ipynb`.
  - Conducts Exploratory Data Analysis (EDA), including:
    - Scatter matrix visualization for feature relationships.
    - Heatmaps for correlation analysis.
  - Applies clustering techniques (e.g., K-Means, DBSCAN) to identify anomalous nodes.
  - Visualizes clustering results to distinguish normal and anomalous behavior.

## 📊 Dataset Details
- **Source:** Social network dataset (e.g., Facebook user interaction data).
- **Structure:**
  - Nodes represent individual users.
  - Edges represent relationships (friendship, interaction, etc.).
  - Features extracted from `.feat` and `.featnames` files.
- **Size:** Contains thousands of users and network interactions.

## 🚀 Installation & Dependencies
To run this project, ensure you have the following dependencies installed:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn networkx
```

## ▶️ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Anomaly-Detection-Social-Networks.git
   cd Anomaly-Detection-Social-Networks
   ```
2. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Run the notebooks in sequence:
   - **First**, run `Adetection.ipynb` to generate `anomaly_features.csv`.
   - **Then**, run `Aclusterning.ipynb` for clustering-based anomaly detection using the generated dataset.
4. Analyze the results using visualizations and model evaluations.

## 📈 Results & Insights
- **Feature-Based Detection:**
  - Flags users exhibiting irregular patterns.
  - Evaluates anomalies with precision and recall metrics.
- **Clustering Approach:**
  - Groups users based on network attributes.
  - Identifies outlier clusters with anomalous nodes.

## 🔮 Future Improvements
- Implement deep learning models for anomaly detection (e.g., Graph Neural Networks).
- Integrate real-time anomaly detection on streaming social network data.
- Optimize feature engineering for enhanced model accuracy.



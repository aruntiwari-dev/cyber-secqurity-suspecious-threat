# 🔐 Cybersecurity: Suspicious Web Threat Interactions

A machine learning project to detect and analyze suspicious web traffic behavior using AWS CloudWatch data.

## 📌 Project Overview

This project focuses on identifying potential cyber threats in real-time by analyzing web traffic logs using various data analysis (DA), feature analysis (FA), and machine learning (ML) techniques.

> **Objective**: Detect suspicious or malicious patterns in web server traffic to strengthen threat detection mechanisms in cloud infrastructure.

---

## 🧠 Technologies Used

- **Languages**: Python, SQL, Excel  
- **Libraries**: `pandas`, `matplotlib`, `seaborn`, `sklearn`, `tensorflow`, `networkx`  
- **Tools**: VS Code, Jupyter Notebook  
- **Models**:
  - Isolation Forest (Anomaly Detection)
  - Random Forest Classifier (Binary Classification)
  - Neural Networks (Deep Learning)

---

## 📂 Dataset

The dataset comprises web traffic logs collected via AWS CloudWatch. Each entry represents a web server interaction and includes metadata such as source/destination IPs, port, protocol, bytes in/out, country codes, and detection rule names.

🔗 [Download Dataset from Google Drive](https://drive.google.com/file/d/1-OpnR9FK8EqGuLFB1k45ctPbl-vuZnC-/view?usp=sharing)

---

## 🧪 Workflow

### 1. Data Preprocessing
- Missing value handling
- Type conversion (timestamp fields)
- Text standardization
- Feature engineering (`session_duration`, `avg_packet_size`)

### 2. Exploratory Data Analysis (EDA)
- Distribution analysis of bytes_in and bytes_out
- Protocol usage patterns
- Detection types by country
- Suspicious activity by port

### 3. Feature Engineering
- Standardization using `StandardScaler`
- One-Hot Encoding for categorical features
- Duration calculation

### 4. Modeling
- **Isolation Forest** for unsupervised anomaly detection
- **Random Forest Classifier** for binary classification
- **Neural Network (Sequential + Conv1D)** models to classify suspicious activity

### 5. Visualization
- Time-series traffic visualization
- Heatmaps of correlation matrices
- Graph plots of IP interactions using NetworkX
- Stacked bar charts of detection type frequency by country

---

## 📊 Model Results

| Model                 | Accuracy  |
|----------------------|-----------|
| Isolation Forest      | -         |
| Random Forest         | **100%**  |
| Neural Network (Dense)| **100%**  |
| Conv1D + Dense NN     | **100%**  |

---

## 📈 Sample Outputs

- Anomalies in web traffic clearly visualized with scatterplots
- Detection of targeted traffic from specific country codes
- Activity spike on non-standard ports indicating potential intrusions
- Feature-rich visual EDA for domain understanding

---

## 🔍 Example Use Cases

- Cloud-based real-time threat detection
- Suspicious behavior analytics in enterprise environments
- Rule enhancement for Web Application Firewalls (WAFs)
- Building alerting systems for DevSecOps pipelines

---

## 📬 Contact
- ### Author: Arun Tiwari
- 📧 Email: aruntiwari1639@gmail.com
- 🔗 LinkedIn/GitHub: [(https://github.com/aruntiwari-dev)]

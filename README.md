# 📡 Indoor Localization using Graph Neural Networks (GNN)

## 📦 Dataset Selection

Indoor location determination using wireless signals is a challenging problem, especially compared to outdoor positioning like GPS. This is due to:

- Multipath propagation
- Non-line-of-sight issues
- Dynamic indoor environments

📍 Traditional GPS performs poorly indoors, which has led to increasing interest in **signal fingerprinting** methods using:

- **Wi-Fi**
- **5G**
- **Bluetooth**

These techniques aim to provide accurate user localization in complex indoor environments such as:

- Shopping malls 🛍️  
- Airports ✈️  
- Subway stations 🚇  

### 🔍 Dataset Overview

This dataset contains:

- **RSSI (Received Signal Strength Indicator)** values from **4 Wi-Fi Access Points (APs)**
- **3D position labels**: (x, y, z) coordinates for each measurement

---

## 🧠 Why This Dataset is Suitable for GNNs

This dataset can be **naturally modeled as a graph**, making it ideal for Graph Neural Networks (GNNs).

| Graph Component | Representation |
|------------------|----------------|
| **Nodes**        | Each (x, y, z) position |
| **Edges**        | Euclidean distances between nearby positions |
| **Node Features**| RSSI values from 4 APs |

### ✅ Advantages of GNN-based Modeling

- **Spatial Awareness**: GNNs can aggregate signal information from neighboring nodes
- **Robustness to Noise**: Helps mitigate noisy or missing RSSI values
- **Generalization**: Learns from the structure of indoor space, not just signal strength

📌 Unlike traditional models that treat each sample independently, GNNs leverage local structure to enhance prediction accuracy in complex and dynamic environments.

---

## 🚀 Applications

- Indoor navigation apps
- Smart building systems
- Location-based services (LBS)

---

> 📁 If you're using this project or dataset, feel free to contribute or cite the original source.

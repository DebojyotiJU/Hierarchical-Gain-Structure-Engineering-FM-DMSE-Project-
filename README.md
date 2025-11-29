# Hierarchical-Gain-Structure-Engineering-FM-DMSE-Project-
Hierarchical Gain Structure Engineering (FM-DMSE Project)  > A physics-guided ML project that generates synthetic gain-engineered materials, computes interaction-matrix descriptors, and trains a multi-task LightGBM model for predicting formation energy and magnetic behavior in crystalline compounds.
# 🧭 Hierarchical Gain Structure Engineering (FM-DMSE Project)

**Author:** [Debojyoti Singha]  
**Department:** [Metallurgical and Material Engineering]  
**Institute:** [JADAVPUR UNIVERSITY]  
**Project Type:** [Final Major Project (FM-DMSE)]  


---

## 🧠 Overview

This repository implements a **data-driven machine learning framework** for  
**Hierarchical Gain Structure Engineering**, focused on understanding how **strain** and **doping** affect the **magnetic and thermodynamic stability** of crystalline materials.

The project is inspired by *Interaction-Matrix-based Magnetic Materials Discovery* (Computational Materials Science, 2026), extending the concept into a **multi-scale, physics-guided ML workflow**.

---

## ⚙️ Features

✅ Fetches real magnetic materials data directly from the **Materials Project API**  
✅ Generates **synthetic gain structures** by applying ±3 % strain and 5 % random atomic doping  
✅ Constructs **interaction-matrix descriptors** representing atomic-level pairwise interactions  
✅ Trains a **multi-task LightGBM regression model** for formation energy & magnetic moment  
✅ Visualizes **feature importance**, **PCA clusters**, and **strain-gain response curves**  
✅ Includes a full **Google Colab notebook** for reproducibility  

---



## 🧱 Methodology

| Step | Description |
|------|--------------|
| **1. Data Acquisition** | Fetched real materials data (formula, structure, formation energy, magnetization) via the Materials Project API using an API key. |
| **2. Gain Structure Generation** | Applied lattice strain (−3 %, 0 %, +3 %) and low-fraction doping to simulate modified “gain” structures. |
| **3. Descriptor Construction** | Built atomic interaction-matrix features combining elemental and pairwise distance properties. |
| **4. Model Training** | Used **LightGBM** multi-output regression to jointly predict formation energy & magnetic moment. |
| **5. Visualization & Interpretation** | Generated feature-importance plots, PCA projections, and gain-vs-strain trends. |

---



## 🧮 Model Performance

| Property | R² Score | RMSE |
|-----------|-----------|------|
| Formation Energy (eV/atom) | 0.88 – 0.91 | ≈ 0.04 |
| Magnetic Moment (μB) | 0.82 – 0.86 | ≈ 0.17 |

> Multi-task regression jointly captures thermodynamic and magnetic trends, enabling efficient screening of gain-engineered materials.

---

## ⚙️ Environment Setup

### 1️⃣ The Repository
git clone https://github.com/<your-username>/Hierarchical-Gain-Structure-Engineering-FM-DMSE-Project.git
cd Hierarchical-Gain-Structure-Engineering-FM-DMSE-Project

### 2️⃣ Install Dependencies
pip install -r requirements.txt

### 3️⃣ Run the Colab / Jupyter Notebook
Open:
notebooks/Hierarchical_Gain_Structure_Engineering.ipynb  
and execute cells sequentially.

---

## 📚 Dataset Information

All source materials data are retrieved from the  
Materials Project Database (https://materialsproject.org/) using their public REST API.  
Synthetic structural variations (strain & doping) are generated programmatically via **pymatgen**.

---

## 🧾 Dependencies

pandas  
numpy  
lightgbm  
scikit-learn  
matplotlib  
seaborn  
pymatgen  
mp-api  
tqdm  
plotly  

Install them automatically with:
pip install -r requirements.txt

---

## 📘 Citation

*Hierarchical Gain Structure Engineering via Multi-Scale Interaction Descriptors*  
Inspired by: “Accelerating Magnetic Materials Discovery using Interaction-Matrix-Based Descriptors”  
Computational Materials Science (2026)

---

## 🧑‍💻 Author’s Note

This project was developed as part of the **Final Major Project (FM-DMSE)** coursework.  
The pipeline merges physics-based descriptors with data-driven insights to support  
**rational design of magnetic materials** through strain and doping engineering.

---

⭐ **If you find this project useful, please give it a star on GitHub!**

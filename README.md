# **DeepFusion-SMAs: Predicting Martensitic Transformation Temperature (Ms) in Multicomponent Shape Memory Alloys**  

## 📌 Overview  
This repository contains the dataset and implementation of a **hybrid deep learning framework (Deep Fusion)** for predicting the **martensitic transformation start temperature (Ms)** in **multicomponent shape memory alloys (SMAs)**. The project integrates **Convolutional Neural Networks (CNNs), Long Short-Term Memory networks (LSTMs), and Transformer models** to analyze complex relationships between alloy composition, thermomechanical processing conditions, and phase transformation temperatures.

## 🗂 Contents  
- 📂 **Dataset/** – Contains experimental and literature-based data on SMA transformation temperatures.  
- 📓 **COMMAT-D-25-00345.ipynb** – Jupyter Notebook implementing the Deep Fusion model for Ms prediction.  
- 📜 **README.md** – This document explaining the project structure and objectives.  

## 🏗 Model Architecture  
The Deep Fusion model combines:
- **CNNs** for extracting spatial patterns from material composition data.  
- **LSTMs** for capturing sequential dependencies in processing conditions.  
- **Transformers** for modeling global relationships among features.  
- **A regression head** to predict Ms temperature accurately.  

## 📊 Dataset Details  
The dataset comprises **32 features**, including:
- **Alloy composition:** Ni, Ti, Hf, Zr, Cu, Pd, Co, Nb.  
- **Mechanical & physical properties:** Bulk modulus, atomic radius, melting temperature, thermal conductivity.  
- **Thermodynamic properties:** Mixing entropy (∆Smix), mixing enthalpy (∆Hmix), valence electron concentration (Cv).  
- **Processing conditions:** Homogenization time/temp, aging time/temp, applied stress.  
- **Transformation temperatures:** Ms, Mf, As, Af.  

## 🚀 How to Use  
1. Clone this repository:  
   ```bash
   git clone https://github.com/your-username/DeepFusion-SMAs.git
   cd DeepFusion-SMAs

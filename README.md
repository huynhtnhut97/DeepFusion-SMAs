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
   jupyter notebook COMMAT-D-25-00345.ipynb

📈 Results
- Achieved a Mean Absolute Error (MAE) of 11.26°C (train set) and 20.16°C (test set).
- Feature importance analysis identified aging temperature, Ti content, and entropy parameters as key factors influencing Ms.
- The model generalizes well but requires additional high-temperature data for further improvements.

🎯 Future Work
- Incorporate more extensive datasets to enhance model accuracy.
- Explore graph neural networks (GNNs) to better model alloy interactions.
- Deploy as an interactive web-based prediction tool.
  
📝 Citation

Huynh, T. N., Raji, H., Saedi, S., & Nguyen, K. D. (2025). 
Deep Learning Framework for Accurate Prediction of Phase Transformation in Multicomponent Shape Memory Alloys. 
(Under review at Computational Materials Science).


🤝 Contributions & Contact
Contributions are welcome! For questions, reach out via email.


# DeepFusion-SMAs: Predicting Phase Change Temperature in Shape Memory Alloys

## 📌 Overview
This repository provides a **hybrid deep learning model** to predict the **martensitic transformation start temperature (Ms)** in **multicomponent shape memory alloys (SMAs)**. The **DeepFusion model** combines neural networks to analyze alloy composition, processing conditions, and material properties, achieving high accuracy. It includes a comprehensive dataset of 32 alloy characteristics to support predictions despite limited data.

## 🗂 Contents
- 📂 **Dataset/** – Experimental and literature data on SMA transformation temperatures.
- 📓 **COMMAT-D-25-00345.ipynb** – Jupyter Notebook with the DeepFusion model implementation.
- 📜 **requirements.txt** – List of Python dependencies for running the project.
- 📜 **README.md** – This file explaining the project structure and goals.

## 🏗 Model Architecture
The DeepFusion model includes:
- **Dense Branch**: Processes alloy properties and processing conditions with neural layers.
- **Self-Attention Branch**: Captures interactions among alloy elements (e.g., nickel, titanium).
- **Regression Head**: Combines outputs to predict Ms temperature accurately.

## 📊 Dataset Details
The dataset includes **32 characteristics**:
- **Alloy composition**: Nickel, titanium, hafnium, zirconium, copper, palladium, cobalt, niobium.
- **Processing conditions**: Homogenization temperature/time, aging temperature/time, applied stress.
- **Material properties**: Atomic mass, bulk modulus, melting temperature, thermal conductivity.
- **Thermodynamic properties**: Mixing entropy, mixing enthalpy, valence electron concentration.

## 🛠 Requirements
Install dependencies using the provided `requirements.txt`:
```bash
pip install -r requirements.txt
```

## 🚀 How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/DeepFusion-SMAs.git
   cd DeepFusion-SMAs
   ```
2. Install dependencies (see Requirements section).
3. Run the notebook:
   ```bash
   jupyter notebook COMMAT-D-25-00345.ipynb
   ```

## 📈 Results
- Achieved a test Mean Absolute Error of 17.22°C and R² of 0.94 (full dataset).
- Analysis shows nickel group (nickel, palladium, copper, cobalt) and aging temperature as key predictors.
- Model excels in complex alloys but needs more high-temperature data for further gains.

## 🎯 Future Work
- Expand dataset with more alloy samples to boost accuracy.
- Explore graph-based neural networks for alloy interactions.
- Develop a web tool for interactive Ms predictions.

## 📝 Citation
Huynh, T. N., Raji, H., Saedi, S., & Nguyen, K. D. (2025). Deep Learning Framework for Accurate Prediction of Phase Transformation in Multicomponent Shape Memory Alloys. (Under review at Computational Materials Science).

## 🤝 Contributions & Contact
We welcome contributions! Open issues or pull requests for improvements. For questions, contact nhuynh2023@my.fit.edu.

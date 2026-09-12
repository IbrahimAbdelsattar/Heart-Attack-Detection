<br/><br/>

<!-- Animated Title -->
<p align="center">
  <a href="#">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=34&pause=1000&color=E11D48&center=true&vCenter=true&width=820&lines=Heart+Attack+Risk+Prediction+%E2%9D%A4%EF%B8%8F%E2%80%8D%F0%9FA9%B9;MLP+Neural+Network+%C2%B7+CDC+Cardiovascular+Indicators;Clinical+Comorbidity+Profiling+%C2%B7+Lifestyle+Biomarkers;Real-Time+Diagnostic+Risk+Score+%C2%B7+Streamlit+Studio" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <b>Production Clinical Machine Learning System for Cardiovascular Event Likelihood Assessment</b><br/>
  <i>Multi-Layer Perceptron (MLP) Neural Network · Multi-Factor Comorbidity Modeling · CDC Heart Disease Indicators · Interactive Streamlit Clinical Studio</i>
</p>

<br/>

<!-- Badges Row 1: Core Technologies -->
<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python Version" />
  <img src="https://img.shields.io/badge/Neural_Network-Scikit--Learn_MLP-EE4C2C?style=for-the-badge&logo=scikitlearn&logoColor=white" alt="MLP Neural Network" />
  <img src="https://img.shields.io/badge/Interface-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit" />
  <img src="https://img.shields.io/badge/Pandas-Data_Frames-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
  <img src="https://img.shields.io/badge/DevContainer-VS_Code-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="DevContainer" />
</p>

<!-- Badges Row 2: Clinical Standards & License -->
<p align="center">
  <img src="https://img.shields.io/badge/Data_Source-CDC_BRFSS_Surveillance-0284C7?style=for-the-badge" alt="CDC Indicators" />
  <img src="https://img.shields.io/badge/Pipeline-End--to--End_Joblib_Bundle-7C3AED?style=for-the-badge" alt="Joblib Bundle" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="License" />
  <img src="https://img.shields.io/badge/Status-Production_Ready-brightgreen?style=for-the-badge" alt="Status" />
</p>

<br/>

<!-- Quick Navigation Bar -->
<p align="center">
  <a href="#-overview"><img src="https://img.shields.io/badge/📌-Overview-E11D48?style=flat-square" alt="Overview" /></a>
  &nbsp;
  <a href="#-problem-statement--clinical-solution"><img src="https://img.shields.io/badge/🎯-Problem%20%26%20Solution-2563EB?style=flat-square" alt="Problem" /></a>
  &nbsp;
  <a href="#-clinical-feature-domains"><img src="https://img.shields.io/badge/🔥-Clinical%20Features-D97706?style=flat-square" alt="Features" /></a>
  &nbsp;
  <a href="#%EF%B8%8F-system-architecture"><img src="https://img.shields.io/badge/🏗️-Architecture-0891B2?style=flat-square" alt="Architecture" /></a>
  &nbsp;
  <a href="#-machine-learning-pipeline"><img src="https://img.shields.io/badge/🔬-ML%20Pipeline-7C3AED?style=flat-square" alt="Pipeline" /></a>
  &nbsp;
  <a href="#-quickstart--execution"><img src="https://img.shields.io/badge/🚀-Quickstart-4F46E5?style=flat-square" alt="Quickstart" /></a>
</p>

---

## 📌 Overview

**Heart Attack Detection** is a clinical decision-support machine learning system engineered to assess the probability of acute myocardial infarction (heart attack) based on comprehensive personal, behavioral, and clinical comorbidity indicators.

Trained on the **CDC Behavioral Risk Factor Surveillance System (BRFSS)** epidemiological dataset, the system deploys a **Multi-Layer Perceptron (MLP) Neural Network** encapsulated within an end-to-end scikit-learn preprocessing pipeline (`mlp_model.pkl`). The accompanying **Streamlit Clinical Studio** enables primary care clinicians, occupational health officers, and individuals to simulate cardiovascular risk profiles across dozens of interdependent health variables.

```
                      ┌────────────────────────────────────────────────────────┐
                      │             Cardiovascular Risk Engine                 │
                      │                                                        │
[ Patient Profile:   ]┼──> [ Pipeline Preprocessor & One-Hot Encoder ]         ├──> [ Diagnostic Risk Score ]
[ Lifestyle & History]│             │                                          │    - Probability (%)
                      │             ▼                                          │    - Binary Classification
                      │    [ Multi-Layer Perceptron (MLP) ] ──> Risk Logits    │    - Stratified Risk Tier
                      │             │                                          │    - Clinical Guidance
                      │             ▼                                          │
                      │    [ Calibrated Sigmoid Output ]    ──> Clinical Risk  │
                      └────────────────────────────────────────────────────────┘
```

---

## 🎯 Problem Statement & Clinical Solution

<table>
<tr>
<td width="50%" valign="top">

### ❌ The Cardiovascular Disease Burden

Cardiovascular diseases remain the leading cause of mortality worldwide:

- ⏳ **Asymptomatic Progression**: Atherosclerosis and hypertension develop quietly over decades without acute symptoms until a cardiac event occurs.
- 🧩 **Multi-Factorial Complexity**: Risk is not determined by a single biomarker but by the compounding synergy of smoking, diabetes, age, BMI, and prior stroke/angina.
- 📋 **Fragmented Screening**: Routine health screenings often lack accessible predictive tools that synthesize lifestyle data into actionable risk metrics.

</td>
<td width="50%" valign="top">

### ✅ The Machine Learning Solution

| Challenge | Architectural Solution |
| :--- | :--- |
| **Synergistic Risk Modeling** | **MLP Neural Network**: Deep interconnected hidden layers capture non-linear interactions across diverse clinical factors. |
| **Comprehensive Feature Scope** | Encodes **Demographics**, **Lifestyle Factors**, **Chronic Comorbidities**, and **Physical Health Metrics**. |
| **Serialized Pipeline Bundle** | **Self-Contained Joblib Pipeline** (`mlp_model.pkl`) managing one-hot encoding, imputation, and inference in one call. |
| **Interactive Clinical Studio** | **Streamlit** multi-column dashboard with specialized clinical categories and instant probabilistic assessment. |

</td>
</tr>
</table>

---

## 🔥 Clinical Feature Domains

<table>
<tr>
<td width="33%" align="center" valign="top">

### 👤 Lifestyle & Demographics
<br/>
<b>Behavioral Factors</b>
<p align="left">
• Age bracket & biological sex<br/>
• Smoker status & E-cigarette usage<br/>
• Alcohol consumption habits<br/>
• Physical activity frequency<br/>
• Sleep duration & mental health days
</p>

</td>
<td width="33%" align="center" valign="top">

### 🏥 Comorbidities
<br/>
<b>Medical History</b>
<p align="left">
• Prior Angina / CAD diagnosis<br/>
• History of Stroke<br/>
• Chronic Kidney Disease<br/>
• Diabetes mellitus diagnosis<br/>
• Asthma, COPD & Arthritis
</p>

</td>
<td width="33%" align="center" valign="top">

### 📊 Vital Biomarkers
<br/>
<b>Physical Health</b>
<p align="left">
• Body Mass Index (BMI)<br/>
• Height and weight ratios<br/>
• Mobility & concentration difficulties<br/>
• Annual checkup recency<br/>
• General health self-rating
</p>

</td>
</tr>
</table>

---

## 🏗️ System Architecture

```mermaid
graph TD
    subgraph ViewLayer["User Interface (Streamlit Clinical Dashboard)"]
        UI["Clinical Form (app0.py)"]
        LifestyleCol["Personal & Lifestyle Information"]
        MedicalCol["Medical History & Comorbidities"]
        DisabilityCol["Mobility & Daily Life Factors"]
        VitalsCol["Health Measurements & BMI"]
    end

    subgraph PipelineCore["Inference Pipeline (mlp_model.pkl)"]
        DataframeAssembler["Pandas DataFrame Assembler"]
        Preprocessor["ColumnTransformer & One-Hot Categorical Encoder"]
        MLP["Multi-Layer Perceptron Neural Network (MLPClassifier)"]
    end

    subgraph ClinicalOutput["Diagnostic Assessment"]
        RiskScore["Heart Attack Probability (%)"]
        AlertStatus["Stratified Risk Category Alert"]
    end

    LifestyleCol --> DataframeAssembler
    MedicalCol --> DataframeAssembler
    DisabilityCol --> DataframeAssembler
    VitalsCol --> DataframeAssembler
    
    DataframeAssembler --> Preprocessor
    Preprocessor --> MLP
    MLP --> RiskScore
    RiskScore --> AlertStatus
```

---

## ⚙️ Technical Stack

| Component | Technology | Purpose & Implementation |
| :--- | :--- | :--- |
| **Neural Network** | **Scikit-Learn MLPClassifier** | Multi-layer perceptron with backpropagation and non-linear activations |
| **Preprocessing Pipeline** | **Scikit-Learn Pipeline** | Unified categorical encoding and feature alignment |
| **Interactive Interface** | **Streamlit** | Multi-column clinical risk prediction dashboard |
| **Data Structures** | **Pandas & NumPy** | Vectorized patient record assembly and feature extraction |
| **Model Serialization** | **Joblib** | Serialized model and pipeline bundle (`mlp_model.pkl`) |
| **Dataset Source** | **CDC BRFSS** | CDC Heart Disease Indicators epidemiological dataset |

---

## 📁 Repository Structure

```
Heart-Attack-Detection/
├── 📄 app0.py                          # Interactive Streamlit clinical risk prediction application
├── 📄 diabetes-eda-and-detection (1).ipynb # Comprehensive EDA, feature selection & training notebook
├── 📄 mlp_model.pkl                    # Serialized MLP neural network pipeline bundle
├── 📊 diabetes_prediction_dataset (1).csv # Training and evaluation dataset
├── 📄 Requirements.txt                 # Dependencies
├── 📁 .devcontainer/                   # Development container configuration
└── 📄 README.md                        # Documentation
```

---

## 🚀 Quickstart & Execution

### Prerequisites
- **Python**: 3.10 or higher
- **Virtual Environment**: Recommended

---

### 1. Installation

```bash
# 1. Clone repository
git clone https://github.com/IbrahimAbdelsattar/Heart-Attack-Detection.git
cd Heart-Attack-Detection

# 2. Create virtual environment
python -m venv venv
source venv/bin/activate        # On Windows: .\venv\Scripts\activate

# 3. Install dependencies
pip install -r Requirements.txt
pip install streamlit scikit-learn pandas numpy joblib
```

---

### 2. Launching the Clinical Dashboard

```bash
streamlit run app0.py
```

*The application will boot at `http://localhost:8501`.*

---

## 👥 Author & Connect

**Ibrahim Abdelsattar**  
*AI Engineer & Machine Learning Specialist*

- 🌐 **GitHub**: [@IbrahimAbdelsattar](https://github.com/IbrahimAbdelsattar)
- 💼 **LinkedIn**: [Ibrahim Abdelsattar](https://www.linkedin.com/in/ibrahim-abdelsattar/)
- 📧 **Email**: [ibrahimabdelsattar042@gmail.com](mailto:ibrahimabdelsattar042@gmail.com)

---

<p align="center">
  <sub>Engineered for clinical intelligence, preventive medicine, and cardiovascular health analytics. © 2026 Heart Attack Detection.</sub>
</p>

# Medical Appointment No-Show Predictor

## 🎯 Project Overview

This project develops a machine learning classifier to predict whether patients will attend their scheduled medical appointments, achieving **85.3% accuracy**. By identifying patients likely to miss appointments, healthcare providers can implement targeted interventions to reduce no-show rates and improve healthcare delivery efficiency.

## 📊 Dataset

**Source**: [Attendance of Medical Appointments in Brazil - Kaggle](https://www.kaggle.com/datasets/catherinenewcomb/attendance-of-medical-appointments-in-brazil)

The dataset contains **110,527 medical appointments** from Brazilian healthcare facilities with 14 features:

### Features Description:
- **PatientId** - Unique identifier for each patient
- **AppointmentID** - Unique identifier for each appointment  
- **Gender** - Patient gender (Male/Female)
- **ScheduledDay** - Date when appointment was scheduled
- **AppointmentDay** - Date of the actual appointment
- **Age** - Patient age
- **Neighbourhood** - Location where appointment takes place
- **Scholarship** - Whether patient participates in [Bolsa Família](https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia) welfare program (1/0)
- **Hypertension** - Patient has hypertension (1/0)
- **Diabetes** - Patient has diabetes (1/0) 
- **Alcoholism** - Patient has alcoholism (1/0)
- **Handicap** - Patient has disability (1/0)
- **SMS_received** - Patient received SMS reminder (1/0)
- **No-show** - **Target variable**: Patient missed appointment (1/0)

## 🔍 Problem Statement

Medical appointment no-shows are a significant challenge in healthcare systems worldwide, leading to:
- **Resource waste** and reduced clinic efficiency
- **Increased healthcare costs** 
- **Delayed care** for other patients
- **Revenue loss** for healthcare providers

This project aims to predict no-show probability to enable proactive interventions such as targeted reminders, overbooking strategies, and patient outreach programs.

## 🛠️ Methodology

### Data Analysis & Preprocessing
- Exploratory data analysis to identify patterns
- Feature engineering and data cleaning
- Handling categorical variables and missing values

### Machine Learning Pipeline
- **Algorithm**: Classification models using Scikit-learn
- **Performance**: 85.3% accuracy achieved
- **Evaluation**: Cross-validation and multiple performance metrics
- **Feature Importance**: Analysis of key predictive factors

## 📈 Key Results

- **Model Accuracy**: 85.3%
- **Primary Predictors**: [To be updated based on analysis]
- **Business Impact**: Enables proactive appointment management

## 🔧 Technologies Used

- **Python** - Core programming language
- **Scikit-learn** - Machine learning algorithms
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib/Seaborn** - Data visualization
- **Jupyter Notebook** - Development environment

## 📁 Repository Structure

```
Appointment_NoShow/
├── Appointment_NoShow.ipynb    # Main analysis notebook
├── data/                       # Dataset files
├── README.md                   # Project documentation
└── requirements.txt            # Dependencies (if applicable)
```

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

### Running the Analysis
1. Clone the repository
2. Open `Appointment_NoShow.ipynb` in Jupyter Notebook
3. Run all cells to reproduce the analysis

**For better notebook viewing**: [NBViewer Link](https://nbviewer.org/github/bergerache/Appointment_NoShow/blob/main/Appointment_NoShow.ipynb)

## 💡 Business Applications

- **Healthcare Scheduling**: Optimize appointment scheduling systems
- **Resource Planning**: Better allocation of medical staff and facilities  
- **Patient Engagement**: Targeted intervention strategies
- **Revenue Optimization**: Reduce lost revenue from no-shows

## 🏷️ Tags

`machine-learning` `classification` `healthcare-analytics` `predictive-modeling` `python` `scikit-learn` `data-science`

## 📧 Contact

Feel free to reach out for questions or collaboration opportunities!

---

*This project is part of a comprehensive Healthcare Analytics Suite focused on improving healthcare delivery through data-driven insights.*

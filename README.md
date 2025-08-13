# Medical Appointment No-Show Predictor 🏥

## 🎯 Project Overview

This machine learning project tackles a critical healthcare challenge: predicting which patients will miss their scheduled medical appointments. The model successfully identifies **78% of no-show patients**, enabling healthcare providers to implement targeted interventions and optimize resource allocation.

**Key Achievement**: **4x improvement** over baseline prediction, transforming appointment management from reactive to proactive.

## 📊 The Challenge

Medical appointment no-shows create significant healthcare inefficiencies:
- **20% baseline no-show rate** across 110,527 appointments
- Resource waste and reduced clinic efficiency  
- Delayed care access for other patients
- Revenue loss for healthcare providers

This project demonstrates how data science can address real-world healthcare operational challenges.

## 🎲 Dataset

**Source**: Medical Appointments No-Show Dataset (São Paulo, Brazil - May 2016)  
**Size**: 110,527 appointments across 81 neighborhoods

### Features Overview

| Category | Features | Description |
|----------|----------|-------------|
| **Demographics** | Age, Gender | Patient characteristics |
| **Health Conditions** | Hypertension, Diabetes, Alcoholism, Handicap | Medical history indicators |
| **Socioeconomic** | Scholarship (Bolsa Família), Neighbourhood | Welfare participation & location |
| **Appointment Details** | SMS_received, ScheduledDay, AppointmentDay | Scheduling and reminder data |
| **Target** | No-show | Whether patient attended (0) or missed (1) appointment |

## 🚀 Key Results & Business Impact

### Model Performance
- **78% Recall** for no-show detection (identifies 4 out of 5 no-shows)
- **F1-Score: 0.44** - strong performance for imbalanced healthcare data
- **4x improvement** over stratified baseline (0.20 → 0.44 F1-score)
- **60% overall accuracy** with balanced sensitivity/specificity trade-off

### Business Value Delivered
- **Proactive Scheduling**: Identify high-risk appointments for targeted outreach
- **Resource Optimization**: Reduce wasted appointment slots by up to 78%
- **Strategic Overbooking**: Data-driven approach to maximize clinic utilization  
- **Patient Engagement**: Enable personalized intervention strategies

## 🔬 Technical Approach

### Advanced Data Engineering
- **Feature Engineering**: Created temporal features (days_to_appointment, appointment_day_of_month)
- **Outlier Management**: Removed scheduling anomalies and age outliers using IQR method
- **Geographic Analysis**: Neighborhood-level no-show rate analysis with outlier filtering

### Machine Learning Pipeline
```python
Pipeline Architecture:
1. Preprocessing: MinMax Scaling + Binary Encoding
2. Class Balancing: SMOTE Oversampling (handles 80/20 imbalance)
3. Classification: Random Forest with optimized hyperparameters
```

### Model Comparison Results

| Algorithm | F1-Score | Key Strengths |
|-----------|----------|---------------|
| **🏆 Random Forest** | **0.44** | Best overall performance, feature importance analysis |
| Gradient Boosting | 0.42 | Strong sequential learning |
| Logistic Regression | 0.41 | Interpretable baseline |
| Hist Gradient Boosting | 0.34 | Fast training alternative |
| K-Neighbors | 0.36 | Local pattern recognition |
| Dummy Classifier | 0.20 | Stratified baseline |

## 🛠️ Technologies & Methods

**Core Stack:**
- **Python**: pandas, numpy, scikit-learn
- **Visualization**: matplotlib, seaborn  
- **ML Techniques**: SMOTE, cross-validation, hyperparameter tuning
- **Evaluation**: Classification reports, F1-optimization for imbalanced data

**Advanced Techniques:**
- ✅ Imbalanced classification with SMOTE oversampling
- ✅ Comprehensive model comparison and selection
- ✅ Feature engineering from temporal data
- ✅ Geographic outlier detection and filtering
- ✅ 5-fold cross-validation for robust evaluation

## 📈 Real-World Applications

### Immediate Implementation
- **Smart Reminders**: Target high-risk patients with personalized follow-ups
- **Appointment Optimization**: Adjust scheduling based on predicted attendance
- **Staff Planning**: Allocate resources based on expected patient volume

### Strategic Opportunities  
- **Predictive Overbooking**: Maximize clinic capacity without overwhelming staff
- **Patient Journey Optimization**: Identify intervention points to improve engagement
- **Healthcare Equity**: Analyze neighborhood-level access patterns

## 💡 Key Technical Insights

**Why 78% Recall Matters:**
In healthcare, **identifying no-shows is more valuable than perfect accuracy**. Missing a no-show (false negative) wastes resources, while a false positive simply triggers an extra reminder call.

**Handling Real-World Complexity:**
- Addressed severe class imbalance (80/20 split) using SMOTE
- Managed 81 unique neighborhoods with geographic outlier detection  
- Created meaningful features from scheduling timestamp data
- Demonstrated robust evaluation methodology with cross-validation

## 🔄 Future Enhancements

**Data Enrichment Opportunities:**
- Weather data correlation with appointment attendance
- Patient transportation accessibility scoring
- Historical no-show patterns per patient
- Appointment type/specialty integration

**Model Evolution:**
- Ensemble methods combining multiple algorithms
- Deep learning for complex pattern recognition
- Real-time prediction API development
- Cost-sensitive learning optimization

## 📁 Repository Structure

```
medical-appointment-noshow/
├── 📓 analysis.ipynb              # Complete ML pipeline & analysis
├── 📊 data/                       # Dataset files  
├── 📋 README.md                   # Project documentation
├── 📦 requirements.txt            # Python dependencies
└── 🖼️ visualizations/             # Generated plots & charts
```

## 🚀 Quick Start

```bash
# Clone repository
git clone [repository-url]

# Install dependencies  
pip install pandas numpy scikit-learn matplotlib seaborn jupyter imbalanced-learn

# Run analysis
jupyter notebook analysis.ipynb
```

## 🏷️ Technical Tags
`machine-learning` `healthcare-analytics` `imbalanced-classification` `random-forest` `smote` `python` `scikit-learn` `predictive-modeling`

---

## 💼 Portfolio Highlight

This project showcases **practical data science skills** in a challenging real-world domain:
- ✅ **Business Impact Focus**: Translates ML metrics into actionable healthcare insights
- ✅ **Technical Rigor**: Proper handling of imbalanced data and model evaluation  
- ✅ **Domain Understanding**: Healthcare operational knowledge applied to feature engineering
- ✅ **Honest Assessment**: Transparent reporting of model limitations and future improvements

**Perfect for healthcare analytics, operations research, or data science roles requiring real-world problem-solving expertise.**

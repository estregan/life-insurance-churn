# Life Insurance Customer Churn Prediction

## 📋 Project Overview

This project develops a comprehensive customer churn prediction system for life insurance policies, demonstrating advanced data engineering techniques and critical data quality analysis.

### Key Highlights
- 🎯 **Objective**: Predict customer churn in life insurance to enable proactive retention strategies
- 📊 **Dataset**: 50,000+ customer records from Kaggle
- 🔍 **Critical Finding**: Identified data quality issues (perfect AUC indicating data leakage)
- 💡 **Value**: Demonstrates importance of data validation and critical thinking in ML projects

## 🚀 Technical Achievements

### Memory Optimization
- Reduced memory usage by **75%** through dtype optimization
- Processed full dataset without sampling using vectorized operations
- Implemented efficient categorical encoding strategies

### Data Engineering
- **PII Detection & Removal**: Automated identification and exclusion of personal information
- **Feature Engineering**: Created 10+ insurance-specific features
- **Class Imbalance**: Handled with class weights instead of SMOTE for memory efficiency

### Model Development
- Implemented multiple algorithms (Logistic Regression, XGBoost)
- Achieved perfect AUC (1.0) - identified as data leakage issue
- Built complete ML pipeline with scaling and preprocessing

## 📊 Results & Analysis

### Model Performance
| Model | AUC | Precision | Recall | F1-Score |
|-------|-----|-----------|--------|----------|
| Logistic Regression | 1.00* | 1.00* | 1.00* | 1.00* |
| XGBoost | 1.00* | 1.00* | 1.00* | 1.00* |

*Perfect scores indicate data quality issues in the dataset

### Business Impact Analysis
- Implemented ROI calculator for retention campaigns
- Optimal threshold analysis for business decision-making
- Cost-benefit analysis framework for interventions

## 🔍 Critical Findings

### Data Quality Issues Identified
1. **Perfect Classification**: Unrealistic 100% accuracy suggests data leakage
2. **Pattern Recognition**: Multiple independent analyses confirmed the issue
3. **Synthetic Data Indicators**: Patterns too clean for real-world data

### Lessons Learned
- ✅ Always validate data quality before modeling
- ✅ Question suspiciously perfect results
- ✅ Cross-reference findings with other practitioners
- ✅ Real-world churn typically achieves 0.65-0.85 AUC

## 🛠️ Technical Stack

- **Language**: Python 3.8+
- **ML Libraries**: Scikit-learn, XGBoost, LightGBM
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Platform**: Google Colab
- **Version Control**: Git/GitHub

## 📁 Project Structure

```
life-insurance-churn/
│
├── README.md                           # Project documentation
├── requirements.txt                    # Python dependencies
├── .gitignore                         # Git ignore file
│
├── notebooks/
│   ├── life_insurance_churn_analysis.ipynb    # Main analysis notebook
│   └── data_quality_investigation.ipynb       # Data leakage analysis
│
├── src/
│   ├── data_preprocessing.py         # Data cleaning and preparation
│   ├── feature_engineering.py        # Feature creation functions
│   ├── model_training.py            # Model training pipeline
│   └── business_metrics.py          # ROI and business calculations
│
├── reports/
│   ├── data_quality_report.md       # Detailed analysis of data issues
│   └── model_performance.md         # Model evaluation results
│
└── docs/
    ├── lessons_learned.md            # Key takeaways
    └── next_steps.md                 # Future improvements
```

## 💻 Installation & Usage

### Prerequisites
- Python 3.8 or higher
- Google Colab account (for notebook execution)
- Kaggle account (for dataset access)

### Setup
```bash
# Clone repository
git clone https://github.com/estregan/life-insurance-churn.git
cd life-insurance-churn

# Install dependencies
pip install -r requirements.txt

# Set up Kaggle API
# Place kaggle.json in ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
```

### Running the Analysis
1. Open `notebooks/life_insurance_churn_analysis.ipynb` in Google Colab
2. Upload your `kaggle.json` when prompted
3. Run all cells sequentially

## 📈 Key Insights

### Technical Optimizations
- **Memory Reduction**: 75% through dtype optimization
- **Processing Speed**: Full dataset processing without sampling
- **Scalability**: Vectorized operations throughout

### Business Value
Despite data quality issues, the project demonstrates:
- Complete ML pipeline development
- Business-focused metrics and ROI analysis
- Critical thinking in result validation
- Production-ready code structure

## 🎯 Skills Demonstrated

- **Data Engineering**: Memory optimization, PII handling, vectorization
- **Machine Learning**: Classification, imbalanced learning, model evaluation
- **Critical Thinking**: Data quality assessment, anomaly detection
- **Business Acumen**: ROI analysis, intervention strategies
- **Software Engineering**: Clean code, documentation, version control

## 📝 Future Improvements

1. **Alternative Datasets**: Test pipeline with validated datasets
2. **Advanced Features**: Survival analysis, customer lifetime value
3. **Model Deployment**: API development for real-time predictions
4. **Monitoring**: Drift detection and model performance tracking

## 👤 Author

**[Your Name]**
- GitHub: [@estregan](https://github.com/estregan)
- Email: your.email@example.com

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Dataset source: [Kaggle - Customer Churn Dataset for Life Insurance](https://www.kaggle.com/datasets/usmanfarid/customer-churn-dataset-for-life-insurance-industry)
- Inspiration from insurance industry best practices
- Google Colab for computational resources

---

**Note**: This project identified significant data quality issues in the dataset (perfect classification accuracy), making it an excellent case study in the importance of data validation and critical thinking in machine learning projects.

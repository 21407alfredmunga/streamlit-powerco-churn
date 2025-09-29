# PowerCo Customer Churn Analysis Dashboard ⚡

An interactive Streamlit dashboard for analyzing customer churn patterns in the energy sector, built as part of a comprehensive data science project exploring customer behavior and retention strategies.

## 🎯 Project Overview

This project analyzes customer churn for PowerCo, an energy company, using machine learning techniques and interactive visualizations. The dashboard provides insights into customer behavior, identifies high-risk segments, and explores the relationship between customer profitability and churn likelihood.

## 🚀 Features

### Interactive Dashboard
- **Real-time Filtering**: Filter customers by gas subscription, number of active products, and acquisition channel
- **Key Metrics**: Live calculation of customer count, churn rate, and average net margin
- **Multi-dimensional Analysis**: 
  - Churn rates by acquisition channel
  - Customer profitability vs. consumption analysis
  - Cohort analysis by activation year
- **Data Explorer**: View and sort filtered customer data

### Visualizations
- Bar charts showing churn probability by acquisition channel
- Scatter plots with marginal distributions for consumption vs. margin analysis
- Stacked bar charts for cohort analysis
- Interactive filtering and drill-down capabilities

## 📊 Data Science Pipeline

The project includes comprehensive Jupyter notebooks covering:

1. **Exploratory Data Analysis** (`BCG X- EDA .ipynb`)
   - Data quality assessment
   - Feature distribution analysis
   - Correlation analysis

2. **Feature Engineering** (`BCG X-Feature engineering.ipynb` & `BCG X-1engineering.ipynb`)
   - Feature creation and transformation
   - Data preprocessing
   - Feature selection

3. **Predictive Modeling** (`BCG X-taskmodelling.ipynb`)
   - Machine learning model development
   - Model evaluation and validation
   - Performance metrics analysis

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **Data Analysis**: Pandas, NumPy
- **Visualization**: Plotly Express
- **Machine Learning**: Scikit-learn, TensorFlow/Keras
- **Development Environment**: Jupyter Notebooks
- **Package Management**: pip, virtual environment

## 📦 Installation & Setup

### Prerequisites
- Python 3.8+
- pip package manager

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/21407alfredmunga/streamlit-powerco-churn.git
   cd streamlit-powerco-churn
   ```

2. **Set up virtual environment** (recommended)
   ```bash
   # Create virtual environment
   python -m venv datascience_env
   
   # Activate virtual environment
   # On Linux/Mac:
   source datascience_env/bin/activate
   # On Windows:
   # datascience_env\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the dashboard**
   ```bash
   streamlit run app.py
   ```

5. **Access the application**
   Open your browser and navigate to `http://localhost:8501`

### Alternative Setup Script
For automated environment setup, you can use the provided script:
```bash
chmod +x create_datascience_env.sh
./create_datascience_env.sh
```

## 📁 Project Structure

```
streamlit-powerco-churn/
├── app.py                          # Main Streamlit dashboard
├── requirements.txt                # Python dependencies
├── create_datascience_env.sh      # Environment setup script
├── data/                          # Dataset files
│   ├── clean_data_after_eda.csv  # Processed data for dashboard
│   ├── Customer_Churn_Data_Large.csv
│   └── ...                       # Raw and intermediate data files
├── notebooks/                     # Jupyter notebooks
│   ├── BCG X- EDA .ipynb         # Exploratory Data Analysis
│   ├── BCG X-Feature engineering.ipynb
│   ├── BCG X-1engineering.ipynb   # Feature engineering
│   └── BCG X-taskmodelling.ipynb # ML modeling
└── datascience_env/              # Virtual environment (created after setup)
```

## 📈 Key Insights & Analysis

The dashboard reveals several important patterns:

- **Acquisition Channel Impact**: Different customer acquisition channels show varying churn rates
- **Product Portfolio Effect**: Customers with multiple active products tend to have different churn patterns
- **Profitability vs. Retention**: Analysis of the relationship between customer value and retention
- **Temporal Patterns**: Cohort analysis showing how customer behavior varies by activation period

## 🔍 Usage Guide

### Dashboard Navigation

1. **Sidebar Filters**:
   - **Gas Subscription**: Filter by customers with/without gas subscriptions
   - **Number of Active Products**: Adjust range slider to focus on specific customer segments
   - **Acquisition Channel**: Select specific marketing channels

2. **Main Dashboard Sections**:
   - **Key Metrics**: Overview of filtered customer base
   - **Channel Analysis**: Churn rates by acquisition method
   - **Profitability Analysis**: Interactive scatter plot with consumption vs. margin
   - **Cohort Analysis**: Customer retention by activation year
   - **Data Explorer**: Detailed view of filtered customer records

### Interpreting the Visualizations

- **Red color gradients** typically indicate higher churn risk
- **Scatter plot size** represents maximum power consumption
- **Marginal plots** show distribution patterns for key metrics
- **Stacked bars** separate active vs. churned customers

## 🔬 Data Science Methodology

### Analysis Framework
1. **Data Exploration**: Understanding data quality, distributions, and relationships
2. **Feature Engineering**: Creating meaningful predictors from raw data
3. **Model Development**: Building and validating predictive models
4. **Dashboard Development**: Creating interactive tools for stakeholder engagement

### Key Datasets
- Customer demographics and contract information
- Consumption patterns and billing data
- Product subscription details
- Historical churn labels

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📝 License

This project is part of a data science portfolio. Please refer to the repository license for usage terms.

## 👤 Author

**Alfred Munga**
- GitHub: [@21407alfredmunga](https://github.com/21407alfredmunga)
- Project: PowerCo Customer Churn Analysis

## 🙏 Acknowledgments

- BCG X Data Science Program for project framework
- PowerCo dataset for enabling comprehensive churn analysis
- Streamlit community for excellent documentation and examples

---

**Note**: This dashboard is built for analytical and educational purposes. The insights generated should be validated with domain expertise before implementation in production environments.
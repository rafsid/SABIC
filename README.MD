# Remote Work Impact Analysis

## Overview
This repository contains a comprehensive causal analysis of the impact of remote work on employee productivity at OptimaTech Solutions. The analysis uses advanced statistical methods including propensity score matching and causal inference frameworks to understand how remote work arrangements affect employee performance and productivity.

## Key Features
- Causal analysis using DoWhy framework
- Propensity score matching for treatment effect estimation
- Multiple regression analyses for robustness checks
- Comprehensive data visualization
- Counterfactual analysis

## Data Description
The analysis uses a synthetic dataset with 1000 employees containing:
- Demographic information (age, gender, marital status, number of children)
- Work-related metrics (department, tenure, remote work status)
- Performance indicators (productivity score, engagement score)
- Communication patterns
- Distance from office

## Technical Stack
- Python 3.x
- Key Libraries:
  - DoWhy for causal inference
  - Pandas for data manipulation
  - Scikit-learn for machine learning components
  - Statsmodels for statistical analysis
  - Seaborn and Matplotlib for visualization

## Methodology
1. **Data Preprocessing**
   - One-hot encoding of categorical variables
   - Standardization of continuous variables
   - Missing value analysis

2. **Causal Analysis**
   - Treatment: Remote Work Status
   - Outcome: Productivity Score
   - Confounders: Demographics, work arrangements, and engagement metrics

3. **Model Validation**
   - Refutation testing using random common cause
   - Data subset refutation
   - Multiple regression analyses
   - Propensity score matching validation

## Key Findings
1. Remote work shows a positive causal effect on productivity:
   - Average Treatment Effect (ATE): ~7.14 points increase in productivity
   - Statistically significant (p < 0.001)
   - Robust across different estimation methods

2. Counterfactual Analysis Results:
   - Mean productivity for all-remote scenario: 70.99
   - Mean productivity for all-onsite scenario: 63.88
   - Difference confirms positive impact of remote work

## Repository Structure
```
├── data/
│   └── synthetic_people_analytics_data_excel.xlsx
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_causal_analysis.ipynb
│   └── 03_counterfactual_analysis.ipynb
├── src/
│   ├── data_preprocessing.py
│   └── causal_analysis.py
├── results/
│   └── transformed.csv
└── README.md
```

## Getting Started
1. Clone the repository:
   ```bash
   git clone https://github.com/username/remote-work-impact-analysis.git
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the analysis:
   ```bash
   jupyter notebook notebooks/01_data_preprocessing.ipynb
   ```

## Requirements
- Python 3.8+
- DoWhy
- Pandas
- NumPy
- Scikit-learn
- Statsmodels
- Seaborn
- Matplotlib

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
For any queries regarding this analysis, please open an issue in the repository.

## Acknowledgments
- OptimaTech Solutions for the project initiative
- DoWhy framework developers for the causal inference tools

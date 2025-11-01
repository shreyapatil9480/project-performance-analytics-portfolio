# Project Performance Analytics Portfolio

Which customers are likely to churn?

**Stakeholder:** Customer Success Lead

## Key Insights

- Tenure under 6 months doubles churn risk for basic-tier accounts.
- Support ticket volume above 5 is a leading churn indicator.
- Premium tier churn is driven more by ticket severity than volume.

## Dataset

Primary file: `data/customer_tenure.csv`  
Target variable: `churned`

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook notebooks/analysis.ipynb
```

## CLI Usage

```bash
python src/train.py
python src/predict.py --input data/sample_input.csv
```

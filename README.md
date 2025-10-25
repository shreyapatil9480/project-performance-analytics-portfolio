# Synthetic Project Performance Analysis

This repository contains a fully self‑contained project designed to showcase **business analytics and data analysis** skills for roles such as *Business Analyst*, *Program Manager*, and *Data Analyst*.  It includes a synthetic dataset, a reproducible Jupyter notebook for exploratory data analysis and predictive modeling, and a `requirements.txt` file specifying the dependencies.  The repository is ready to run out of the box.

## Repository Contents

| File | Description |
|------|-------------|
| `synthetic_project_data.csv` | A synthetic dataset of 200 project records covering programs, start/end dates, planned vs. actual durations and budgets, team sizes, stakeholder satisfaction scores, and a binary `success` outcome indicating whether the project finished on time, under budget, and with high satisfaction. |
| `project_analysis.ipynb` | A Jupyter notebook that loads the dataset, performs exploratory data analysis with summary statistics, correlation analysis, and visualizations (histograms, scatter plots, heatmaps), and builds a logistic regression model to predict project success. |
| `requirements.txt` | A list of Python packages required to run the notebook. |

## Dataset Details

The synthetic dataset simulates project performance metrics commonly encountered in program management.  Each row represents a single project with the following fields:

- `project_id` – Unique project identifier (PRJ0001, PRJ0002, …).
- `program` – High‑level program category (Program A–D).
- `start_date` – Project start date.
- `end_date` – Project end date (calculated from `start_date` + actual duration).
- `planned_duration_days` – Planned duration in days.
- `actual_duration_days` – Actual duration in days.
- `planned_budget` – Planned budget (USD).
- `actual_cost` – Actual cost (USD).
- `team_size` – Number of people assigned to the project.
- `stakeholder_satisfaction` – Stakeholder satisfaction score (1–10 scale).
- `success` – Binary flag indicating whether the project finished on time and within budget with a satisfaction score > 6.

Although the data are synthetic, they are generated with realistic ranges and variability to approximate challenges faced by project and program managers.  The success flag provides a clear target variable for predictive modeling.

## Quick Start

1. **Clone or download** this repository from GitHub.
2. Ensure you have the dependencies listed in `requirements.txt` installed.  You can install them using pip:

   ```bash
   pip install -r requirements.txt
   ```

3. Launch the Jupyter notebook:

   ```bash
   jupyter notebook project_analysis.ipynb
   ```

4. **Run through the notebook** to explore the data, visualize key relationships, and build a logistic regression model to predict project success.  The notebook includes comments explaining each step.

## Extending the Project

- **Additional Models:** You can experiment with other algorithms (e.g., decision trees, random forests, gradient boosting) to compare predictive performance.
- **Feature Engineering:** Introduce new features such as cost variance (actual–planned), duration variance, or categorical encodings of programs.
- **Dashboarding:** Build a dashboard using tools like Tableau or Power BI to present insights to stakeholders.
- **Time Series Analysis:** Create a time series forecast of project cost over time or analyze trends by program.

This project is intentionally designed to be adaptable to your interests.  By modifying the dataset or analysis, you can highlight skills relevant to the roles you’re targeting.

## License

This project is provided under the MIT License.  Feel free to use and adapt it for your portfolio or learning purposes.

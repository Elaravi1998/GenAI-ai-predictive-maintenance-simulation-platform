# AI Predictive Maintenance & Simulation Platform

An end-to-end Python reference project for industrial predictive maintenance. It generates synthetic equipment telemetry, trains a failure-risk classifier, recommends maintenance actions, and compares maintenance policies through a what-if simulation.

## Features
- Synthetic daily sensor data for pumps, motors, and compressors
- Rolling-window sensor feature engineering
- Random Forest model for 7-day failure-risk classification
- Asset risk bands and maintenance recommendations
- Sensor trend and asset-risk visualizations
- What-if maintenance policy simulation
- CSV and JSON report exports

## Workflow
1. Generate synthetic telemetry.
2. Engineer sensor and rolling features.
3. Train and evaluate the classifier.
4. Score assets and recommend actions.
5. Simulate baseline and preventive-maintenance policies.
6. Export reports.

## Repository structure
```text
ai-predictive-maintenance-simulation-platform/
├── ai_predictive_maintenance_simulation_platform.ipynb
├── README.md
└── requirements.txt
```

## Getting started
```bash
git clone https://github.com/YOUR_USERNAME/ai-predictive-maintenance-simulation-platform.git
cd ai-predictive-maintenance-simulation-platform
python -m venv .venv
```
Activate the environment:

Windows PowerShell:
```powershell
.venv\Scripts\Activate.ps1
```
macOS/Linux:
```bash
source .venv/bin/activate
```
Install and launch:
```bash
pip install -r requirements.txt
jupyter notebook
```
Open `ai_predictive_maintenance_simulation_platform.ipynb` and run all cells.

## Technology stack
Python, Jupyter Notebook, pandas, NumPy, scikit-learn, Matplotlib.

## Outputs
The notebook creates `outputs/` with:
- `asset_risk_recommendations.csv`
- `maintenance_policy_simulation.csv`
- `maintenance_report.json`

## Limitations and responsible use
This is an educational prototype using synthetic data. It is not validated for real industrial equipment or safety-critical use. Failure labels, risk thresholds, costs, and intervention-effect assumptions are illustrative. The random split is not a substitute for time-based and asset-based validation. Qualified reliability engineers must review any real-world maintenance decision. Do not connect this prototype to control systems or automatically shut down equipment.

## Future enhancements
- Real IoT/historian data ingestion
- Remaining useful life estimation
- Time-series validation and probability calibration
- SHAP explanations and model-drift monitoring
- Streamlit dashboard and CMMS integration with human approval

## License
Choose and add a license before distributing this repository.

#  Predictive Maintenance - Engine Health Monitor

##  Project Overview
This capstone project develops a **predictive maintenance system** using engine sensor data.  
The goal is to classify whether an engine is operating normally or requires maintenance, helping reduce breakdowns, optimize schedules, and improve reliability.

##  Objectives
- Reduce unplanned breakdowns and costly repairs.
- Improve vehicle performance and engine lifespan.
- Optimize maintenance schedules to minimize downtime.
- Provide actionable insights for manufacturers and fleet operators.

##  Repository Structure
/data          → raw dataset (engine_data.csv), train/test splits
/notebooks     → Jupyter notebooks (EDA, preprocessing, model training)
/models        → saved models (best_model.pkl), model card
/deployment    → Dockerfile, requirements.txt, Streamlit app, hosting script
/ci-cd         → GitHub Actions pipeline.yml
/reports       → interim_report.md, final_report.md
README.md      → project overview and instructions

##  Dataset
- **Engine rpm**: Revolutions per minute (RPM)
- **Lub oil pressure**: Pressure of lubricating oil (bar)
- **Fuel pressure**: Fuel supply pressure (bar)
- **Coolant pressure**: Engine coolant pressure (bar)
- **Lub oil temp**: Lubricating oil temperature (°C)
- **Coolant temp**: Engine coolant temperature (°C)
- **Engine Condition**: Binary label (0 = Normal, 1 = Faulty)

##  Workflow
1. **Data Registration** → Upload dataset to Hugging Face Datasets.
2. **EDA** → Explore sensor patterns and correlations.
3. **Data Preparation** → Clean, normalize, split into train/test.
4. **Model Building** → Train ML models (Decision Tree, Random Forest, XGBoost).
5. **Experiment Tracking** → Log parameters and metrics.
6. **Model Deployment** → Streamlit app + Docker + Hugging Face Spaces.
7. **CI/CD Automation** → GitHub Actions pipeline for reproducibility.
8. **Business Insights** → Recommendations for cost savings and reliability.

##  Deployment
- Interactive **Streamlit app** with sliders for RPM, pressures, and temperatures.
- Real‑time prediction: Normal  vs Faulty .
- Probability visualization with a risk gauge.

##  Business Impact
By implementing predictive maintenance:
- Fleet operators can reduce downtime.
- Manufacturers gain data‑driven insights.
- Owners save on costly repairs and extend engine lifespan.

---


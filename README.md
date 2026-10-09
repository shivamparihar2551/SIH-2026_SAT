# SAT-SA — Supervisory Analytics Tool for SOC Assessment

SAT-SA is a data-driven cybersecurity supervision platform designed to analyze SOC operations, assess security analyst behavior, and identify unusual operational patterns using rule-based intelligence and machine learning.

## Key Features

- **Data Ingestion:** Load and manage security datasets using CSV and PostgreSQL.
- **Analyst Performance Analytics:** Calculate alert-handling metrics, investigation activity, closure times, evidence-review rates, and escalation rates.
- **Rule-Based Risk Assessment:** Identify potentially concerning behavioral patterns using configurable detection rules.
- **Machine Learning Anomaly Detection:** Apply the Isolation Forest algorithm with feature standardization to identify analysts whose behavior differs from the broader population.
- **Risk Intelligence:** Generate risk scores, anomaly scores, and indicators to support supervisory review.
- **Scalable Data Processing:** Process multiple interconnected datasets using SQLAlchemy and grouped SQL aggregations.

## Technology Stack

- **Language:** Python
- **Database:** PostgreSQL
- **Data Processing:** SQLAlchemy, NumPy
- **Machine Learning:** Scikit-learn, Isolation Forest, StandardScaler
- **Backend Framework:** FastAPI
- **Frontend:** React

## Project Objective

The objective of SAT-SA is to transform SOC operational data into actionable supervisory insights by combining statistical analysis, predefined behavioral rules, and unsupervised machine learning. The platform is intended to support human-led investigation and assessment rather than automatically determine misconduct.

## Current Progress

- PostgreSQL database configured and connected.
- Eight datasets ingested, totaling 200,000 rows.
- Analyst-level metrics and rule-based risk assessment implemented.
- Isolation Forest anomaly detection implemented and tested on sample data.
- Integration of the ML model with PostgreSQL-backed analyst analytics is the next development step.

**Note:** An anomaly indicates an unusual pattern that warrants further review; it does not, by itself, establish wrongdoing.

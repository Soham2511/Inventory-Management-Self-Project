# Cash Flow–Linked Inventory Management System
This repository contains an MVP implementation of a cash flow–linked inventory management system. The project integrates inventory KPIs with the cash conversion cycle (CCC) to highlight liquidity tied up in excess stock and evaluate the impact of optimized reorder policies.

## Features
- Data Input: Upload or use sample CSV files containing SKU-level sales, purchases, lead times, and payment terms.
- KPI Engine: Calculates Days Inventory Outstanding (DIO), Cash Conversion Cycle (CCC), stock turnover, and excess stock value.
- Reorder Policy Simulation: Implements dynamic reorder models (EOQ + buffer stock + lead-time adjustments).
- Dashboard (Streamlit):

## Repository Structure
```bash
inventory_mvp/
│── data/                # Sample datasets (CSV)
│── src/                 # Core logic
│   ├── kpi.py           # Inventory KPIs + Cash Conversion Cycle
│   ├── policy.py        # Reorder policy models
│   └── dashboard.py     # Streamlit frontend
│── results/             # Screenshots, reports
│── requirements.txt     # Python dependencies
│── README.md            # Project documentation
```

## Tech Stack
- Python 3.9+
- Pandas, Numpy (data processing)
- Matplotlib / Plotly (visualization)
- Streamlit (dashboard)
- Scikit-learn (optional: forecasting demand)

## Example Use Case
- Upload historical inventory + sales data.

- Dashboard displays:
  $3M tied up in excess stock across 4 years.
  35% projected stockout reduction with dynamic reorder policy.
  12–16% YoY liquidity improvement from optimized cycles.

## Future work
- Integrate with live ERP/PoS systems.
- Add demand forecasting (ARIMA / Prophet).
- Build an alerting system for cash flow risks.

# Subway Risk Analysis

Monte Carlo simulation for underground metro station construction using Primavera P6, Excel, Power BI, @RISK, and Primavera Risk Analysis. 10,000 iterations, 13 systemic risk factors, and comprehensive dashboard.

---

## Overview

Monte Carlo simulation for an underground metro station construction project in the Middle East. This project demonstrates probabilistic risk analysis for schedule and cost uncertainty in mega infrastructure projects.

---

## Tools Used

### Scheduling
- Primavera P6 – Deterministic schedule (140 activities, resources, costs)
- MS Project – Schedule interoperability demonstration

### Risk Analysis
- Excel – Monte Carlo simulation (10,000 iterations, 3 scenarios)
- @RISK – Validation and sensitivity analysis (tornado charts)
- **Primavera Risk Analysis** – Advanced schedule and cost risk analysis

### Visualization
- Power BI – Interactive dashboard (duration histogram, cost histogram, scenario comparison, S-curves, contingency)

---

## Key Results

### Deterministic (Primavera P6)
| Metric | Value |
|--------|-------|
| Duration | 817 days |
| Direct Cost | $2,022,065 |

### Monte Carlo (Excel – Comprehensive Scenario)
| Metric | Value |
|--------|-------|
| P50 Duration | 1,239 days |
| P80 Duration | 1,257 days |
| P50 Cost | $24.77 million |
| P80 Cost | $25.12 million |
| Cost Contingency | $357,096 |

### Primavera Risk Analysis
| Metric | Value |
|--------|-------|
| P50 Duration | 940 days |
| P80 Duration | 953 days |
| P80 Cost | $2,041,000 |
| Top Risk Drivers | Architectural Finishes (28%), MEP Rough-ins (28%) |

---

## Risk Factors Modeled

13 systemic risks including:

| Risk Factor | Impact Range |
|-------------|--------------|
| War / Geopolitical | 0% to 40% |
| Pandemic | 0% to 35% |
| Supply Chain | 0% to 30% |
| Ground Conditions | 0% to 15% |
| Labor Availability | 0% to 10% |
| Weather | 0% to 15% |
| Regulatory | 0% to 20% |
| Financial | 0% to 15% |
| Design Changes | 0% to 25% |
| Equipment | 0% to 10% |
| Material | 0% to 12% |
| Safety Incident | 0% to 35% (5% probability) |
| Extreme Event | 50% impact (10% probability) |

---

## Primavera Risk Analysis Outputs

- Duration, Cost, and Finish Date Distributions
- Schedule Sensitivity Index
- Cost Sensitivity Index
- Criticality Index
- Cruciality Index
- Scatter Plot (Cost vs Finish Date)
- Probabilistic Cash Flow
- Schedule Check Report
- Risk Register (140 activities)

---

## Files

### Primavera P6
- `Primavera_P6_Export.xer` – Original schedule with resources

### MS Project
- `Primavera_P6_Export.mpp` – MS Project export

### Excel Monte Carlo
- `Monte_Carlo_Simulation_Formulas.xlsx` – Excel simulation with formulas
- `Monte_Carlo_Simulation_Results.xlsx` – Excel simulation with static results

### Power BI
- `PowerBI_Dashboard.pbix` – Interactive dashboard (5 pages)

### Primavera Risk Analysis
- `Primavera_Risk_Analysis/` – Folder with all PRA outputs
  - `PRA_Duration_Distribution.png`
  - `PRA_Cost_Distribution.png`
  - `PRA_Finish_Date_Distribution.png`
  - `PRA_Schedule_Sensitivity_Index.png`
  - `PRA_Cost_Sensitivity.png`
  - `PRA_Criticality_Index.png`
  - `PRA_Cruciality_Index.png`
  - `PRA_Scatter_Plot.png`
  - `PRA_Cash_Flow.png`
  - `PRA_Schedule_Check_Report.pdf`
  - `PRA_Risk_Register.xlsx`

### Screenshots
- `Screenshots/` – All Power BI and software screenshots

---

## Author

Abdullah Tarek
Abdullahtarek.003@gmail.com

---

## License

This project is part of my bachelor thesis at the German University In Cairo ( GUC ).

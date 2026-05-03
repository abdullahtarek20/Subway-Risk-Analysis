# 🚇 Underground Metro Station (UMS) - Risk Analysis Platform

[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://python.org)
[![Streamlit](https://img.shields.io/badge/streamlit-1.28.0-red.svg)](https://streamlit.io)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

**Monte Carlo simulation for underground metro station construction using Primavera P6, Excel, Primavera Risk Analysis (PRA), Python, Power BI, Revit, and MS Project.**

> 🎓 **Bachelor Thesis Project** | German University in Cairo (GUC) | Risk Analysis Using Monte Carlo Simulation

---

## 📋 Table of Contents

- [Overview](#overview)
- [Key Results](#key-results)
- [Tools & Technologies](#tools--technologies)
- [Methodology](#methodology)
- [Risk Factors Modeled](#risk-factors-modeled)
- [Results Comparison](#results-comparison)
- [Project Structure](#project-structure)
- [Installation & Usage](#installation--usage)
- [Validation](#validation)
- [Author](#author)
- [License](#license)

---

## 📌 Overview

This project demonstrates a comprehensive **probabilistic risk analysis** for an underground metro station construction project in the Middle East. The analysis integrates:

- **Revit 3D Model** – Detailed BIM model with material quantities (42,264 m³ concrete)
- **Primavera P6** – Deterministic schedule (140 activities, 1,693 days baseline)
- **Excel Monte Carlo** – Custom spreadsheet model (10,000 iterations, 3 scenarios)
- **Primavera Risk Analysis (PRA)** – Industry-standard validation benchmark
- **Custom Python Software** – Open-source risk analysis tool (original contribution)
- **Power BI** – Interactive dashboard for visualization
- **MS Project** – Schedule interoperability demonstration

### 🎯 Key Achievements

| Achievement | Result |
|-------------|--------|
| **Python Software Validation** | Within 2.3% of PRA for P50 duration ✅ |
| **Correlation Impact** | +61.8% duration increase from independent to comprehensive scenario |
| **Open-Source Alternative** | Free, transparent, extensible risk analysis tool |
| **Comprehensive Risk Model** | 13 systemic risk factors, 10,000 iterations |

---

## 📊 Key Results

### Deterministic Baseline (Primavera P6 + Revit)

| Metric | Value |
|--------|-------|
| **Total Project Duration** | **1,693 days** |
| Number of Activities | 140 |
| Critical Path Activities | ~42 |
| Direct Cost | $51,276,399 |
| Indirect Cost | $12,765,220 |
| **Total Baseline Cost** | **$64,041,619** |
| Indirect Rate | $7,540/day |

### Primavera Risk Analysis (PRA) – Industry Benchmark

| Percentile | Duration (days) | Finish Date | Cost ($) |
|------------|----------------|-------------|----------|
| Deterministic (24/22%) | 1,693 | 23/10/2030 | $64,041,619 |
| **P50** | **1,727** | **25/11/2030** | **$64,192,025** |
| **P80** | **1,817** | **24/02/2031** | **$65,248,704** |
| **P90** | **1,867** | **15/04/2031** | **$65,858,695** |

### Custom Python Software – Original Contribution

| Percentile | Duration (days) | Cost ($) |
|------------|----------------|----------|
| **P50** | **1,766** | **$66,734,894** |
| **P80** | **1,889** | **$70,031,675** |
| **P90** | **1,967** | **$72,340,442** |

### Excel Monte Carlo – Comprehensive Scenario

| Metric | Value |
|--------|-------|
| P50 Duration | 2,943 days |
| P80 Duration | 2,960 days |
| P50 Cost | $69,756,362 |
| P80 Cost | $69,884,961 |

---

## 🛠 Tools & Technologies

| Category | Tools |
|----------|-------|
| **BIM & Modeling** | Autodesk Revit |
| **Scheduling** | Primavera P6, MS Project |
| **Risk Analysis** | Excel, Primavera Risk Analysis (PRA), Python (Custom) |
| **Visualization** | Power BI, Plotly |

---

## 🔬 Methodology

### Three Simulation Scenarios

| Scenario | Description | Risk Factors |
|----------|-------------|--------------|
| **Scenario 1** | Independent durations | None |
| **Scenario 2** | Basic correlation | 5 operational risks |
| **Scenario 3** | Comprehensive correlation | 13 systemic risks |

### Simulation Parameters

| Parameter | Value |
|-----------|-------|
| Monte Carlo iterations | 10,000 |
| Sampling method | Latin Hypercube / Random |
| Activity uncertainty | Triangular distribution |
| Confidence levels | P50, P80, P90 |

### Revit 3D Model Quantities

| Element | Volume (m³) |
|---------|-------------|
| Diaphragm Walls | 10,537 |
| Base Slab (Raft) | 8,512 |
| Intermediate Slabs | 9,856 |
| Roof Slab | 5,914 |
| Columns | 3,536 |
| Excavation | 3,909 |
| **Total Concrete** | **42,264 m³** |

> 🎥 **Revit 3D Model Video** – *[Link to Revit 3D model video will be added here]*

---

## ⚠️ Risk Factors Modeled

### Operational Risks (5 factors)

| Risk Factor | Impact Range | Affected Activities |
|-------------|--------------|---------------------|
| Weather | 0-15% | Excavation, concrete |
| Labor | 0-10% | Concrete, finishing |
| Material | 0-12% | Concrete |
| Ground | 0-15% | Diaphragm, piles, excavation |
| Equipment | 0-10% | Excavation, piles |

### Systemic Risks (8 factors)

| Risk Factor | Impact Range | Affected Activities |
|-------------|--------------|---------------------|
| War / Geopolitical | 0-40% | All material-intensive |
| Pandemic | 0-35% | All on-site |
| Supply Chain | 0-30% | Material-dependent |
| Regulatory | 0-20% | Site work, finishing |
| Financial | 0-15% | All activities |
| Design Changes | 0-25% | Concrete, diaphragm, finishing |
| Safety Incident | 0-35% (5% prob) | Random activities |
| Extreme Event | +50% (10% prob) | Random activities |

---

## 📈 Results Comparison

### Duration Comparison

| Metric | Excel | PRA | Python | Python vs PRA |
|--------|-------|-----|--------|---------------|
| P50 Duration | 2,943 days | 1,727 days | **1,766 days** | **+2.3%** ✅ |
| P80 Duration | 2,960 days | 1,817 days | **1,889 days** | **+4.0%** ✅ |
| P90 Duration | N/A | 1,867 days | **1,967 days** | **+5.4%** ✅ |

### Cost Comparison

| Metric | Excel | PRA | Python | Python vs PRA |
|--------|-------|-----|--------|---------------|
| P50 Cost | $69.76M | $64.19M | **$66.73M** | **+4.0%** ✅ |
| P80 Cost | $69.88M | $65.25M | **$70.03M** | **+7.3%** ✅ |
| P90 Cost | N/A | $65.86M | **$72.34M** | **+9.8%** ✅ |

### Validation Summary

| Metric | Python vs PRA | Classification |
|--------|---------------|----------------|
| P50 Duration | +2.3% | ✅ Excellent |
| P80 Duration | +4.0% | ✅ Excellent |
| P50 Cost | +4.0% | ✅ Excellent |
| P80 Cost | +7.3% | ⚠️ Acceptable |

> **All results within ±10% industry tolerance (AACE International, 2022)**

---

## 📁 Project Structure

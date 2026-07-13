# Government Compliance Analytics Platform

### Microsoft Fabric • Power BI • OneLake • Direct Lake • SQL • AI Chatbot

> A Microsoft Fabric-powered analytics platform that unifies GST, Udyam MSME, DISCOM electricity consumption, survey data, and economic indicators into a single compliance intelligence system for government stakeholders.

---

## Project Overview

Government departments often maintain enterprise data across multiple independent systems.

GST records contain taxation information.

Udyam maintains MSME registrations.

DISCOMs record industrial electricity consumption.

Survey teams capture field verification data.

Although each dataset provides valuable insights, they operate independently, making enterprise-level analysis slow, fragmented, and heavily dependent on manual reconciliation.

This project demonstrates how Microsoft Fabric can be used to integrate these disconnected datasets into a unified analytics platform capable of supporting compliance monitoring, cross-department reconciliation, and enterprise intelligence.

---

## Business Problem

Imagine investigating a manufacturing company.

To understand its compliance status, an officer may need to check:

- GST Portal
- Udyam MSME Portal
- DISCOM records
- Survey reports
- Internal master tables

Every system tells only part of the story.

Without integration:

- enterprise identities cannot be reconciled easily
- investigation requires multiple portals
- inconsistent records remain undetected
- reporting becomes manual
- high-risk enterprises are difficult to prioritize

The challenge was not a lack of data.

The challenge was that the data never spoke to each other.

---

# Solution

This platform creates a centralized analytical layer using Microsoft Fabric.

Instead of analysing each source independently, all enterprise records are standardized, reconciled and modeled into a single semantic layer powering interactive Power BI dashboards.

```

External APIs / Files

↓

Microsoft Fabric Pipelines

↓

OneLake Lakehouse

↓

Bronze → Silver → Gold

↓

SQL Validation & Data Reconciliation

↓

Semantic Model

↓

Power BI (Direct Lake)

↓

Government Dashboards

↓

Compliance Officers

```

---

# Data Sources

The analytical model combines multiple government datasets.

| Dataset | Purpose |
|----------|----------|
| GST | Registration, Returns, Turnover |
| Udyam MSME | Enterprise Registration |
| DISCOM | Electricity Consumption |
| Survey Data | Enterprise Validation |
| NIC Classification | Industry Categorization |
| GSDP / GVA | Economic Benchmarking |
| Internal Master Data | Administrative Mapping |

---

# Dashboard Modules

The report consists of seven analytical modules.

## 1. GSDP / GVA Analysis

Provides the economic context of Andhra Pradesh.

Highlights:

- Gross State Domestic Product
- Gross Value Added
- Sector contribution
- Agriculture vs Industry vs Services
- State economic composition

This page establishes the macro-economic baseline used throughout the report.

---

## 2. MSME Data Overview

This module explains how multiple source systems are reconciled.

Key insights include:

- Total Udyam registrations
- Unique enterprise counts
- Survey coverage
- Mobile-based record matching
- DISCOM CA mapping
- GST linkage statistics
- Validation base creation

This page documents the complete reconciliation pipeline from raw records to the final analytical dataset.

---

## 3. Sector Wise Analysis

Classifies enterprises using NIC codes.

Users can analyse:

- Broad sector distribution
- Industry composition
- GST availability
- Estimated turnover
- Electricity consumption
- DISCOM coverage

This helps identify sectors with stronger or weaker compliance characteristics.

---

## 4. MSME Turnover Insights

Provides detailed turnover analytics.

Features include:

- Enterprise turnover ranking
- Sector-wise turnover
- Estimated turnover
- GST reported turnover
- NIC level comparison
- Udyam vs GST comparison

This module allows analysts to compare reported business activity with estimated enterprise turnover.

---

## 5. GST Insights

Focuses on GST availability and reporting behaviour.

KPIs include:

- GST linked enterprises
- Enterprises without GST
- Over-reported turnover
- Under-reported turnover
- GST collection analysis
- Reporting category distribution

This page supports compliance monitoring rather than compliance determination.

Potential cases requiring further investigation are surfaced through analytical comparisons.

---

## 6. Geographic Intelligence

Provides district-level analysis using Azure Maps.

Users can identify:

- High-risk districts
- Estimated tax gaps
- Under-reported enterprises
- Enterprises without GST registration
- Geographic compliance distribution

Spatial analysis helps officers prioritize investigation efforts regionally.

---

## 7. Year-over-Year Performance

Tracks reporting trends across multiple financial years.

Includes:

- GST collections
- Estimated turnover
- Reporting categories
- Sector comparison
- Fiscal year trends

The objective is to monitor changes in reporting behaviour over time.

---

# Technical Highlights

- Microsoft Fabric Lakehouse
- Medallion Architecture
- Direct Lake Semantic Models
- Power Query
- Advanced DAX
- SQL-based Data Validation
- Cross-source Reconciliation
- Enterprise Data Modeling
- Azure Maps Integration
- Power Apps Workflow Integration

---

# Key Business Capabilities

✔ Enterprise Record Matching

✔ Cross-department Data Integration

✔ GST Linkage Validation

✔ Electricity Consumption Analytics

✔ Estimated Turnover Modelling

✔ Sector Intelligence

✔ District-level Risk Analysis

✔ Self-service Executive Dashboards

---

# Dashboard Preview

## GSDP / GVA Analysis

> State-level economic overview combining GSDP, GVA and sector contribution.

*Screenshot*

---

## MSME Data Overview

> Enterprise reconciliation across Udyam, Survey and DISCOM datasets.

*Screenshot*

---

## Sector Wise Analysis

> Industry-wise distribution using NIC classification.

*Screenshot*

---

## MSME Turnover Insights

> Enterprise turnover analysis and sector benchmarking.

*Screenshot*

---

## GST Insights

> GST linkage, reporting behaviour and turnover validation.

*Screenshot*

---

## Geographic Intelligence

> District-wise compliance monitoring using Azure Maps.

*Screenshot*

---

## Year-over-Year Analysis

> Multi-year comparison of GST and estimated turnover.

*Screenshot*

---

# Technology Stack

| Category | Technologies |
|-----------|-------------|
| Analytics | Power BI |
| Data Platform | Microsoft Fabric |
| Storage | OneLake |
| Modeling | Semantic Models |
| ETL | Data Pipelines |
| Query | SQL |
| Transformation | Power Query |
| Measures | DAX |
| Reporting | Direct Lake |
| Workflow | Power Apps |
| APIs | REST APIs |

---

# Repository Structure

```
Government-Compliance-Analytics/

│

├── README.md

├── docs/

│ ├── 01-Business-Problem.md

│ ├── 02-Business-Objectives.md

│ ├── 03-Data-Sources.md

│ ├── 04-Solution-Architecture.md

│ ├── 05-Data-Model.md

│ ├── 06-Reconciliation-Logic.md

│ ├── 07-Power-BI-Dashboard.md

│ ├── 08-DAX-Measures.md

│ ├── 09-Business-Impact.md

│ └── 10-Lessons-Learned.md

│

├── Screenshots/

├── pbix/

└── assets/

```

---

# Key Takeaways

This project demonstrates how Microsoft Fabric can unify multiple government datasets into a centralized analytics platform capable of supporting compliance monitoring, enterprise intelligence, and executive decision making.

Rather than replacing investigation, the platform enables officers to spend less time collecting data and more time analysing it.

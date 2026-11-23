# NetPulse Rwanda
## Telecommunications Network Performance and Service Quality Monitoring System

**Student Name:** Uhiriwe Benajamin  
**Student ID:** 20251SEN298  
**Course:** INSY 8311 – Database Development with PL/SQL  
**Academic Year:** 2026–2027  
**Instructor:** Eric Maniraguha  
**Repository:** https://github.com/pivoben/uhiriwe_20251sen298_netpulse

---

## 1. Project Overview

NetPulse Rwanda is a proposed telecommunications network performance and service quality monitoring system designed using Oracle Database and PL/SQL.

The project aims to organize and analyze real-world internet performance measurements to understand network service quality across different geographical locations and reporting periods in Rwanda.

The system will focus on three network performance indicators:

- Download speed
- Upload speed
- Network latency

Using these measurements, the system will help users compare network performance, identify areas with poor measured performance, monitor historical trends, and generate performance reports.

The proposed primary data source is Ookla Speedtest Open Data. Rwanda coverage, dataset size, selected reporting periods, and applicable licence terms must be verified before the dataset is finalized.

## 2. Problem Statement

Internet connectivity is important for education, businesses, communication, and digital services in Rwanda.

However, internet performance can vary between geographical locations and over time. Slow download speeds, low upload speeds, and high network latency can affect the quality of online services.

Without an organized database system for storing, comparing, and analyzing network performance measurements, identifying areas with consistently poor measured performance and monitoring changes over time can be difficult.

NetPulse Rwanda proposes an Oracle-based solution for organizing network performance measurements and producing reports to support network service quality analysis.

## 3. Project Objectives

### 3.1 Main Objective

To design and implement a telecommunications network performance and service quality monitoring system using Oracle Database and PL/SQL, based on real-world internet performance measurements relevant to Rwanda.

### 3.2 Specific Objectives

1. Collect and organize real internet performance measurements from an appropriate public dataset.
2. Design and implement a normalized relational database for storing network measurements and geographical information.
3. Develop PL/SQL procedures, functions, cursors, and packages for network performance analysis.
4. Implement triggers, exception handling, and auditing to enforce database rules and monitor important operations.
5. Develop an interactive dashboard for visualizing network performance and generating reports.
6. Identify geographical areas with poor measured network performance using documented performance thresholds.

## 4. Data Source

**Proposed primary data source:** Ookla Speedtest Open Data.

- Official repository: https://github.com/teamookla/ookla-open-data

The dataset provides aggregated internet performance measurements that may include:

- Average download speed
- Average upload speed
- Average latency
- Number of speed tests
- Number of unique devices
- Geographic tile information

The project will investigate available mobile and fixed broadband measurements for Rwanda.

The final dataset, reporting periods, record count, licence, file format, and data-quality findings will be documented in `data/dataset_card.md` after the original data has been downloaded and inspected. No dataset size or Rwanda record count is claimed at this stage.

## 5. Planned Database Tables

The following tables are preliminary. They will be finalized after data sourcing, normalization, and ERD development.

| Table | Description |
|---|---|
| `GEOGRAPHIC_AREAS` | Stores geographical area information, where supported by the source data |
| `NETWORK_TYPES` | Stores network categories such as mobile and fixed |
| `REPORTING_PERIODS` | Stores reporting years and quarters |
| `PERFORMANCE_MEASUREMENTS` | Stores download, upload, and latency measurements |
| `QUALITY_THRESHOLDS` | Stores defined network performance thresholds |
| `PERFORMANCE_ALERTS` | Stores generated performance alerts |
| `IMPORT_BATCHES` | Tracks dataset import operations |
| `AUDIT_LOGS` | Records selected database operations |

## 6. Planned PL/SQL Features

| Feature | Planned application |
|---|---|
| Stored procedures | Importing and managing performance measurements |
| Functions | Calculating documented network performance indicators or scores |
| Explicit cursors | Generating geographical performance reports |
| Packages | Organizing network monitoring operations |
| Triggers | Applying documented rules and generating alerts when defined conditions are met |
| Exception handling | Handling invalid measurements and database errors |
| Auditing | Recording important database changes |
| `DBMS_SCHEDULER` | Scheduling periodic performance reporting, if supported by the environment |

## 7. Innovation

The proposed innovation is an interactive network performance monitoring dashboard developed using Oracle Application Express (APEX).

The dashboard is planned to connect to the Oracle database and provide:

- Network performance summaries
- Download and upload speed comparisons
- Latency analysis
- Geographical and reporting-period filters, depending on dataset coverage
- Historical performance trends
- Performance alerts and reports

Business rules and database operations will be implemented in PL/SQL. The dashboard will provide an interactive interface for accessing the results.

The working connection to the Oracle database and the dashboard will be demonstrated during the final project presentation.

## 8. Technologies

| Technology | Purpose |
|---|---|
| Oracle Database 26ai | Database management |
| PL/SQL | Database programming and business logic |
| SQL Developer | Database development and testing |
| Oracle APEX | Proposed interactive dashboard |
| Git and GitHub | Version control and project documentation |
| Ookla Open Data | Proposed real-world dataset |

## 9. Project Development Phases

The project will follow the examination phases:

1. **Phase 0:** Research, Data Source, and Project Proposal.
2. **Phase I:** Business Process Modeling.
3. **Phase II:** Data Sourcing, Normalization, and Logical Design.
4. **Phase III:** Oracle Pluggable Database Creation.
5. **Phase IV:** Tables and Data Loading.
6. **Phase V:** PL/SQL Development.
7. **Phase VI:** Advanced Programming and Auditing.
8. **Phase VII:** Documentation, Innovation, and Final Presentation.

## 10. Repository Structure

```text
netpulse-rwanda/
├── README.md
├── .gitignore
├── data/
│   ├── raw/
│   ├── processed/
│   └── dataset_card.md
├── docs/
│   ├── research/
│   │   └── research_log.md
│   ├── proposal/
│   ├── presentation/
│   └── business_process/
├── database/
│   ├── setup/
│   ├── tables/
│   ├── procedures/
│   ├── functions/
│   ├── packages/
│   ├── triggers/
│   └── auditing/
├── innovation/
│   └── apex/
└── screenshots/
```

## 11. Phase I – Business Process Modeling

This section is reserved for the student's independently completed Phase I work.

- **Selected business process:** To be investigated and documented by the student.
- **Modeling tool:** To be completed by the student.
- **Published diagram link:** To be added by the student.
- **Supporting explanation:** To be added after the student's independent work.

Follow the examination's Phase I instructions and academic-integrity requirements. This README does not supply or generate the required business-process analysis or diagram.

## 12. References

1. Ookla. (n.d.). *Ookla Open Data*. https://github.com/teamookla/ookla-open-data

Additional academic, technical, and institutional references will be added after they have been located, read, and recorded in `docs/research/research_log.md`. Only sources actually consulted should be cited.

---

**Project Author:** Uhiriwe Benajamin  
**Student ID:** 20251SEN298  
**Course:** INSY 8311 – Database Development with PL/SQL  

*NetPulse Rwanda – Measuring Network Performance, Improving Digital Connectivity.*

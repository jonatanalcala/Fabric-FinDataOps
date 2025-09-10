# Fabric-FinDataOps

**Fabric-FinDataOps** is a financial data governance and analytics platform built on **Microsoft Fabric**.  
It demonstrates how financial institutions can manage compliance, automate infrastructure, and deploy machine learning pipelines using synthetic trade data.

---

## Project Roadmap
This project evolves in four phases:

1. **Phase 1 – Governance Framework**  
   - Define compliance requirements (SOX, PCI-DSS, AML, GDPR).  
   - Create a **data contract** for the equity trade blotter dataset.  
   - Map risks to the 6 V’s of Big Data.  

2. **Phase 2 – Cloud Platform Implementation**  
   - Deploy dataset into **Fabric Lakehouse** (`RegulaTrade_Lakehouse`).  
   - Implement role-based access controls (RBAC) and retention policies.  
   - Optimize for scalability and performance.  

3. **Phase 3 – Infrastructure Automation**  
   - Infrastructure-as-Code for Fabric resources.  
   - CI/CD pipelines for dataset + contract deployment.  
   - Monitoring & logging setup.  

4. **Phase 4 – MLOps Pipeline**  
   - End-to-end ML deployment (fraud detection / TCA slippage model).  
   - Automated retraining and monitoring.  
   - Integration with governance policies.  

---

## Dataset
The project uses a **synthetic equity trade blotter dataset** (~1M rows), designed to simulate real-world trading operations.

- **Source:** Generated for this project (not real financial data).  
- **Sample:** [trade_blotter.csv](data/trade_blotter.csv)  
- **Schema:** [trade_blotter_schema.json](data/trade_blotter_schema.json)  
- **Data Contract:** [datacontract.yaml](data/datacontract.yaml)  

---

## Tech Stack
- **Microsoft Fabric** (Lakehouse, OneLake, Notebooks, Power BI)  
- **PySpark & Pandas** (data quality & analytics)  
- **YAML Data Contracts** (governance & compliance)  
- **CI/CD + Infrastructure-as-Code** (automation)  
- **MLOps frameworks** (model deployment & monitoring)  

---

## 📂 Repo Structure
```text
Fabric-FinDataOps/
│── README.md               
│── LICENSE                  
│
├── data/
│    ├── trade_blotter.csv
│    ├── trade_blotter_schema.json
│    └── datacontract.yaml
│
├── notebooks/
│    ├── governance_analysis.ipynb
│    ├── quality_checks.ipynb
│    └── tca_slippage_analysis.ipynb
│
├── infra/
│    ├── fabric_lakehouse_setup.md
│    └── requirements.txt
│
├── docs/
│    ├── Phase1_Governance_Framework.md   
│    ├── Phase2_Cloud_Implementation.md   
│    ├── Phase3_Infrastructure_Automation.md 
│    └── Phase4_MLOps_Pipeline.md        
│
└── reports/
     └── TCA_dashboard.pbix
```

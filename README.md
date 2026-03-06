# Agricultural Supply Chain Simulation: Missouri Soybean Yield Forecast

**A Technical Case Study in API Integration, MS SQL Warehousing, and Random Forest Modeling**

### **Challenge**

Global commodities firms must position logistical assets (barges, trucks, elevators) months before harvest. This project simulates a supply chain intelligence tool designed to predict county-level soybean yields in Missouri, identifying geospatial "High Risk" zones based on climate volatility.

### **Action**

* **Automated Data Pipeline**: Engineered a Python-based ingestion engine to pull 10+ years of historical yield data from the USDA NASS API and corresponding climate records from the NOAA ACIS API.
* **Relational Data Warehousing**: Designed and populated a local MS SQL Server instance to serve as the project's single source of truth, implementing a "Warehouse Cleanup" script to ensure data integrity.
* **Feature Engineering (M.S. Stats Focus)**: To increase model sensitivity, I engineered a **Yield Lag (T-1)** feature and a **Precipitation Volatility** metric, accounting for the impact of "Flash Droughts" on late-summer crop development.
* **Multi-Tool Visualization**: Developed an interactive Plotly choropleth map in Python and a comprehensive Tableau dashboard to identify counties falling below a 42 bu/acre production safety threshold.

### **Result**

The simulation successfully demonstrates how integrating disparate API sources into a predictive model can isolate thermal stress impacts. By identifying "High Risk" zones through a Random Forest Regressor, the project provides a scalable framework for logistical contingency planning.

Analyse data and create Reports/Dashboards

### Types
- **Power BI desktop** - free
- **Power BI service** - premium

##### Difference between Power BI app and service
Dashboard can be created only in power BI service

### ETL
```mermaid

graph TB

0["Extraction (Internal Data source)"] --> 1
1["Transform (Power Query editor- Clean<br>the data)"]
1 --> 2["Load the data"]

style 0 fill:#ba271b
style 1 fill:#457eba
style 2 fill:#434483

```
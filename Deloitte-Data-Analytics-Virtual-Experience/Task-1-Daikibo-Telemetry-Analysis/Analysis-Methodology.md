
# Task 1 – Analysis Methodology

## 1. Understanding the Dataset

The analysis began with understanding the Daikibo telemetry dataset and identifying the information required to examine equipment health and operational downtime.

The dataset was provided in JSON format.

## 2. Data Preparation

The telemetry data was prepared for analysis in Tableau.

The relevant factory, device, and equipment status information was used to develop the required visualizations.

## 3. Calculated Field Creation

A calculated field named `Unhealthy` was created in Tableau.

Formula:

```text
IF [Status] = "unhealthy"
THEN 10
ELSE 0
END
```

### Explanation

- Records with an unhealthy status were assigned a value of 10.
- Records with a healthy status were assigned a value of 0.
- The calculated field was used to quantify unhealthy equipment events for the downtime analysis.

## 4. Factory-Wise Downtime Analysis

A visualization named `Down Time per Factory` was created.

Purpose:
- Examine downtime across different factories.
- Compare factory-level operational performance.
- Identify locations requiring further investigation.

## 5. Device-Type-Wise Downtime Analysis

A visualization named `Down Time per Device Type` was created.

Purpose:
- Compare downtime across equipment categories.
- Examine device-level operational issues.
- Understand the distribution of equipment downtime.

## 6. Dashboard Development

Both visualizations were combined into a Tableau dashboard.

The factory visualization was configured as an interactive dashboard filter.

When a factory was selected, the device-type visualization updated to display the corresponding analysis.

## 7. Analysis and Interpretation

The visualizations were used to examine differences in downtime across factories and device categories.

The dashboard provided a consolidated view of operational performance.

## 8. Final Output

The completed task consisted of two analytical visualizations and an interactive Tableau dashboard.

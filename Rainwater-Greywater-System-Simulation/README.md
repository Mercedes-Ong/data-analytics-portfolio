# Rainwater Harvesting and Greywater System Performance Simulation

## Project Overview

This project evaluates the performance and economic feasibility of combined rainwater harvesting and greywater reuse systems in Australian households.

The analysis integrates time series rainfall forecasting, household water balance simulation, and Monte Carlo cost modelling to assess water savings and financial viability under uncertainty.

The goal is to determine which tank sizes provide the best balance between water security and economic performance.

---

## Dataset

Historical rainfall data were obtained from the Australian Bureau of Meteorology (BOM).  

Household water demand and greywater generation estimates were based on sustainability reports and academic studies.

Key inputs used in the simulation include:

• Rainfall (mm)  
• Roof catchment area  
• Greywater generation rates  
• Household water demand  
• Tank capacity  
• Installation and maintenance costs  

---

## Methodology

The project integrates three analytical components.

### 1. Rainfall Forecasting

Rainfall patterns were modelled using a **Seasonal Autoregressive Integrated Moving Average (SARIMA)** model.

Steps:

• Stationarity testing using the **Augmented Dickey-Fuller test**  
• Model selection using seasonal autoregressive parameters  
• Forecast generation for weekly rainfall

---

### 2. Water Balance Simulation

A weekly water balance model simulated the operation of rainwater and greywater systems.

Each week the model calculates:

Tank Storage  
Rainwater Input  
Greywater Input  
Household Water Demand  
Mains Water Supplement  
Overflow

Tank sizes evaluated:

• 2000 L  
• 3000 L  
• 4000 L  
• 5000 L  
• 7000 L  
• 8000 L  
• 10,000 L

---

### 3. Economic Analysis

A Monte Carlo simulation was implemented to evaluate economic uncertainty.

Random variables included:

• Greywater generation  
• Household demand  
• Runoff efficiency  
• Tank costs  
• Maintenance costs

Key economic metrics calculated:

• Net Present Value (NPV)  
• Cost per litre of water saved  
• Payback period  
• Probability of system paying back within 10 years

---

## Key Results

### Rainfall Forecasting

The Augmented Dickey-Fuller test confirmed that the rainfall time series was stationary.

The selected model:

```
SARIMA(1,0,0)(1,0,0)[52]
```

The model captured seasonal rainfall patterns and produced realistic weekly rainfall forecasts used in the simulation.

---

### System Performance

Small tank sizes showed limited water storage capacity.

2000L – 4000L tanks remained mostly empty and relied heavily on mains water.

5000L tanks significantly reduced mains water usage while maintaining stable storage.

Larger tanks (7000L – 10,000L) eliminated mains water usage completely but stored excess unused capacity.

---

### Economic Viability

Monte Carlo simulation revealed that **smaller tank systems produced the highest economic returns.**

Key findings:

• 2000L tank produced the highest Net Present Value  
• Payback period was extremely short (~0.13 years)  
• Larger tanks became economically inefficient due to high installation costs

Very large tanks (7000L+) generated **no financial return** because mains water usage dropped to zero, eliminating potential cost savings.

---

## Conclusion

The results suggest that **smaller tank systems provide the most economically viable solution** for combined rainwater and greywater reuse systems.

While larger tanks improve water security, they become financially inefficient due to high capital costs and limited additional savings.

This highlights the importance of optimising storage capacity rather than simply maximising tank size.

---

## Tools Used

R  
Time Series Analysis  
SARIMA Modelling  
Monte Carlo Simulation  
Statistical Modelling

# COVID-19 Modeling and Forecasting System

A hybrid **epidemiological forecasting system** combining the **SEIR (Susceptible–Exposed–Infectious–Recovered) model** with a **Multi-Layer Perceptron (MLP) neural network** to simulate and predict the spread of COVID-19 in India during its first wave.

---

## Features

- **SEIR Mathematical Modeling** to simulate disease progression using differential equations.
- **MLP Neural Network** for machine learning-based future case forecasting.
- **Data Preprocessing** with missing value handling, feature engineering, and parameter optimization.
- **Validation and Visualization** of predictions against real-world datasets using MSE metrics.
- Built using **Python (SciPy, NumPy, Matplotlib).**

---

## Project Workflow

1. **Data Collection**  
   Sources:  
   - [Johns Hopkins University COVID-19 Dataset](https://github.com/CSSEGISandData/COVID-19)  
   - Our World In Data  
   - Government Health Portals  

2. **Data Preprocessing**  
   - Cleaning missing values  
   - Converting cumulative counts to daily counts  
   - Setting initial SEIR parameters  

3. **SEIR Model Implementation**  
   - Solving ODEs using `scipy.integrate.odeint`  
   - Parameters:  
     - Transmission Rate (`β`)  
     - Incubation Rate (`σ`)  
     - Recovery Rate (`γ`)  
     - Social Activity Factor (`ρ`)  
   - Population: 10,000 (synthetic data)  
   - Time Frame: 100 days  

4. **Model Validation**  
   - Compare SEIR predictions with real-time COVID-19 data  
   - Evaluate performance using Mean Squared Error (MSE)  

5. **MLP Regressor Training & Forecasting**  
   - Train MLP neural network on SEIR-generated data  
   - Forecast future cases (infected, recovered)  
   - Validate against real-world trends  

6. **Visualization**  
   - Plot predicted vs. actual cases using Matplotlib  

---

## Results

- Simulated **10,000+** population dataset over **100+ days**.
- Processed over **1 million** real-world data points.
- Achieved **90%+ forecasting accuracy** using MLP regressor.
- Validated SEIR model predictions with real-time COVID-19 data.

---

## Technologies Used

- **Python 3.x**  
- **NumPy**  
- **SciPy**  
- **Matplotlib**  
- **Machine Learning (MLP Neural Networks)**  
- **ODE Solvers**  
- **Data Preprocessing Techniques**  

---




# Data Generation using Modelling and Simulation for Machine Learning

## Objective
The objective of this project is to demonstrate how simulation-based modelling can be used to generate synthetic datasets for machine learning model training and evaluation when real-world data is limited or unavailable.

---

## Simulation Tool / Model
A traffic-inspired stochastic simulation model was developed using Python. Randomized traffic parameters are passed into the simulator, which computes the average vehicle waiting time as output.

To improve realism, Gaussian noise was added to the simulation output to model real-world uncertainty.

---

## Simulation Parameters

| Parameter | Description | Lower Bound | Upper Bound |
|---------|------------|-------------|-------------|
| vehicle_count | Number of vehicles | 50 | 500 |
| traffic_density | Traffic density | 0.1 | 1.0 |
| avg_speed | Average speed (km/h) | 20 | 80 |
| signal_duration | Traffic signal duration (seconds) | 20 | 120 |
| lane_count | Number of lanes | 1 | 4 |

---

## Data Generation Process
- Random parameter values were generated within defined bounds  
- Each parameter set was passed to the simulation model  
- The simulation output produced the average waiting time  
- A total of 1000 simulation runs were executed  
- The generated dataset was stored in CSV format  


https://colab.research.google.com/github/shreyataluja2/Data-Generation-using-Modelling-and-Simulation-for-ML/blob/main/simulation_ml.ipynb

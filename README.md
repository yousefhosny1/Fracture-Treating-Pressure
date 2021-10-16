# Fracture-Treating-Pressure
Surface Treating Pressure (STP) Forecast using LSTM in Oil & Gas Drilling Operations

Surface Treating Pressure (STP) is the pressure at the surface during a drilling operation. Surface treating pressure is only controllable through the slurry rate, thus we adjust the slurry rate to increase / decrease the STP. It is important to estimate the STP in order to have enough hydraulic horsepower (HHP) on site during the drilling operation and to predict the required pump power in the given timestep to maintain a specific Surface Treating Pressure.

Slurry is a fluid used in frac fluid, which is the combination of water, chemicals, and sand (or another type of proppant) that is injected at high speeds into a well during hydraulic fracturing (commonly known as fracking) to release the crude oil or natural gas trapped under the earth


In this project I have used a time-series dataset which has the following columns:
    - Time (Seconds)
    - Slurry Rate (Pressure Per Minute)
    - Proppant Concentration (Pounds per Gallon)
    - Surface Treating Pressure (PSI)


Throughout this project I have achieved the following
  1. Handled missing values in the dataset 
  2. Built LSTM Model to forecast the Surface Treating Pressure given the Slurry Rate and Proppant Concentration in the current timestep "Predicting y(t+1) using X(t)".
  2. Explored different window sizes (30, 60, 90, 180 seconds) and their corresponding LSTM Model performance.
  3. Achieved a 20 PSI (Negligable) difference between the final LSTM Model Prediction vs Actual Surface Treating Pressure.

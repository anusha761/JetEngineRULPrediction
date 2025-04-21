# Jet Engine Remaining Useful Life (RUL) Prediction
> This project focuses on predicting the Remaining Useful Life (RUL) of jet engines using time-series sensor data. The primary aim is to support predictive maintenance strategies in the aviation industry, minimizing unplanned downtime, enhancing safety, and optimizing engine performance. The project utilizes an LSTM-based deep learning approach to capture the temporal degradation patterns of turbofan engines, enabling accurate cycle-level RUL forecasts.

## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Contact](#contact)


## General Information
- This project addresses the need for reliable Remaining Useful Life (RUL) estimation for jet engines, a critical aspect of predictive maintenance in the aerospace sector.
- The dataset contains run-to-failure records for 100 turbofan jet engines operating under the same flight condition. Each engine has multiple cycles of time-series sensor readings until it fails. This setup introduces a strong temporal dependency, which was preserved during data preparation.
- A turbofan is a type of jet engine widely used in commercial aircraft, where a large fan drives air through both the engine core and around it to produce thrust efficiently.
- The RUL refers to the number of operating cycles an engine can undergo before it is likely to fail or require major maintenance.
- Data preprocessing involved exploratory data analysis, stationarity testing, and structuring the data into meaningful time-windowed sequences to feed into a deep learning model.
- A Long Short-Term Memory (LSTM) neural network was trained on these sequences to learn temporal degradation patterns and forecast the number of remaining cycles before failure.
- The business objective is to provide aviation operators with a reliable tool for cycle-level RUL prediction, allowing for proactive maintenance scheduling and reduction of unexpected failures.


## Conclusions

- The dataset was sequential in nature, simulating real-world engine wear. the daatset included the sequential data for 100 turbofan engines.
- Stationarity tests were conducted and it was observed that there are non stationary series in many of the sensore readings.
- Proper reshaping and windowing ensured that time dependencies were retained for modeling.
- Sensor behavior over time was explored, and trends relevant to engine degradation were studied through visualizations and statistical testing.
- Data was preprocessed into sliding time windows, and meaningful sequences were created for supervised learning.
- An LSTM model was chosen due to its ability to model time-series dependencies. The model was trained and validated effectively.
- The model achieved an RMSE of 14, which is a reasonable performance threshold in the context of predictive maintenance (typically <20 is considered strong in such simulations).
- The project demonstrates how deep learning can be leveraged for real-time health monitoring and failure forecasting, adding value to industrial asset management systems.


## Technologies Used
- pandas - version 2.2.2
- numpy - version 1.26.4
- matplotlib - version 3.7.1
- seaborn - version 0.13.2
- scikit-learn - version 1.3.1
- tensorflow - version 2.15.0


## Contact
Anusha Chaudhuri – [anusha761]

# Spatial-Temporal Deep Learning Model for Predicting Particulate Matter 2.5 (PM2.5) in Sri Lankan Urban Cities

## Description
This project focuses on predicting air pollution levels, specifically Particulate Matter 2.5 (PM2.5), in urban areas of Sri Lanka. Using spatial-temporal deep learning models, satellite imagery, and sensor data, we aim to develop a comprehensive framework for forecasting PM2.5 levels and identifying potential sources of pollution.

## Usage
1. Run the main script from the relevant model.
2. Follow the prompts to input data and generate predictions.

## Data Sources
- Sensor data collected from 18 stations distributed across Sri Lanka.
- Satellite imagery for spatial analysis and feature extraction.

## File Structure
- `data/`: Directory containing datasets and preprocessing scripts.
- `models/`: Directory containing trained deep learning models and the results gained from each model.
- The final Report of Part I of the project is [here.](https://github.com/IshanBhanuka/FYP-DeepLearningmodel-for-PM2.5/blob/main/G11_EE_405_Report.pdf)

## Models Used
- **ARIMA (AutoRegressive Integrated Moving Average)**: A classical time series forecasting model.
  - Code: [Link to ARIMA code](https://github.com/IshanBhanuka/FYP-DeepLearningmodel-for-PM2.5/blob/main/Model/ARIMA%202%2C1%2C1/Cluster%201/ARIMA%20model%202%2C1%2C1%20cluster%201.ipynb)

- **ETS (Error, Trend, Seasonality)**: A statistical model for time series forecasting.
  - Code: [Link to ETS code](https://github.com/IshanBhanuka/FYP-DeepLearningmodel-for-PM2.5/blob/main/Model/ETS/Cluster%201/ETS%20model%20prediction%20cl1.ipynb)

- **LSTM (Long Short-Term Memory)**: A type of recurrent neural network (RNN) architecture suitable for time series data.
  - Code: [Link to LSTM code](https://github.com/IshanBhanuka/FYP-DeepLearningmodel-for-PM2.5/blob/main/Model/LSTM/LSTM_cluster1_ver3.ipynb)
    
- **GRU (Gated Recurrent Unit)**: Another type of recurrent neural network architecture similar to LSTM but with fewer parameters.
  - Code: [Link to GRU code](/models/gru.py)

- **Random Forest**: An ensemble learning method for classification and regression tasks.
  - Code: [Link to Random Forest code](https://github.com/IshanBhanuka/FYP-DeepLearningmodel-for-PM2.5/blob/main/Model/Random%20Forest/Cluster%201/randomforest%20cl1%20.ipynb)


## Conclusion and Future Work
In our study, various methods for forecasting PM2.5 concentration in 3 clusters were compared. The results show that LSTM is the most accurate and reliable model for PM2.5 prediction for our dataset. We plan to further enhance our machine learning and deep learning models by fine-tuning hyperparameters, exploring different architectures, and incorporating new techniques. Additionally, we aim to develop a hybrid model that combines satellite imagery and advanced deep-learning techniques to predict PM2.5 levels in areas without sensor networks. Continuous monitoring and analysis of air quality patterns will be essential for ensuring the effectiveness and reliability of our predictive models over time.


## Contributing
Contributions are welcome! Please submit bug reports or feature requests via the GitHub issue tracker.


## Acknowledgments
We would like to express our heartfelt gratitude to our supervisor, Dr. Nalin 
Harischandra from the Faculty of Engineering, University of Peradeniya, for his invaluable 
guidance, support, and mentorship which enabled us to complete this project related to course EE 405 – Undergraduate 
project-I on time throughout the process.

## Contact Information
For questions or inquiries, please contact our team,
- [Lahiru Herath](mailto:e18132@eng.pdn.ac.lk)
- [Ishan Bhanuka](https://github.com/IshanBhanuka)
- [Kaushan Nanayakkara](mailto:e18216@eng.pdn.ac.lk)

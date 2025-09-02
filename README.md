# Spatial-Temporal Deep Learning Model for Predicting Particulate Matter 2.5 (PM2.5) in Sri Lankan Urban Cities

## Description
This project focuses on predicting air pollution levels, specifically Particulate Matter 2.5 (PM2.5), in urban areas of Sri Lanka. Using spatial-temporal deep learning models, satellite imagery, and sensor data, we aim to develop a comprehensive framework for forecasting PM2.5 levels and identifying potential sources of pollution.

Project Summary - 
For More info - [Visit Our Website](https://sites.google.com/view/ee405project-e18324/home)

The project was completed in two phases:  
- **Part I:** Focused on temporal prediction using statistical, machine learning, and deep learning approaches.  
- **Part II:** Extended the work with a hybrid **CNN-LSTM model**, integrating temporal features from LSTM with spatial features extracted from satellite images via CNN, resulting in a significant boost in predictive performance.

 

## Data Collection and Clustering
- **Data Sources:**
  - Hourly averaged PM2.5 data from **18 monitoring stations** across Sri Lanka.  
  - Satellite imagery (RGB) for spatial analysis and feature extraction.  
  - Timestamps and geographical metadata for clustering.  

- **Clustering:**
  - Pearson correlation used to group the 18 stations into **3 clusters**, representing regions with similar PM2.5 behavior and air quality patterns. 

## File Structure
- `data/`: Directory containing datasets and preprocessing scripts.
- `models/`: Directory containing trained deep learning models and the results gained from each model.
- The final Report of the project is [here.](https://github.com/IshanBhanuka/FYP-DeepLearningmodel-for-PM2.5/blob/main/G11_EE_406_Report.pdf)


## Models Used

### Part I – Temporal Prediction
- **ARIMA (AutoRegressive Integrated Moving Average)**
  - Code: [Link to ARIMA code](/Model/ARIMA%202%2C1%2C1/Cluster%201/ARIMA%20model%202%2C1%2C1%20cluster%201.ipynb)
- **ETS (Error, Trend, Seasonality)**
  - Code: [Link to ETS code](/Model/ETS)  
- **Random Forest**
  - Code: [Link to Random Forest code](/Model/Random%20Forest)
- **LSTM (Long Short-Term Memory)**
  - Code: [Link to LSTM code](/Model/LSTM/LSTM_cluster1_ver3.ipynb) 
- **GRU (Gated Recurrent Unit)**  
  - Code: [Link to GRU code](/Model/gru_model)

📌 **Key Finding:** LSTM consistently outperformed other models in time-series prediction, making it the most reliable for PM2.5 forecasting.  


### Part II – Spatial & Hybrid Prediction
- **CNN (Convolutional Neural Network)**  
  - Pre-trained **VGG16** used to extract deep features from RGB satellite images.  
  - Handcrafted indices (Green Index, Urban Index, Near-Road Index) were added.  
  - Extracted features passed through fully connected layers for predictions.
  - [Link to CNN code](/Model/CNN%20Models)  

- **Hybrid CNN-LSTM**  
  - LSTM captured the temporal dynamics of PM2.5 data.  
  - CNN extracted spatial patterns from satellite imagery.  
  - Predictions combined using **linear regression** to optimize weight allocation.
  - [Link to Hybrid Model code](/Model/Hybrid%20model/hybrid-ver2.ipynb)  

📌 **Key Finding:** The **Hybrid CNN-LSTM model** achieved the best performance, surpassing standalone models.  


## Results

- **Hybrid CNN-LSTM:**  
  - **R² = 86.86%** → Most accurate and reliable.  

- **CNN only:**  
  - **R² = 83.84%** → Strong performance, captured spatial patterns effectively.  

- **LSTM only:**  
  - **R² = 41.13%** → Less accurate, but useful for temporal insights.  

These results confirm that integrating both spatial and temporal features leads to more robust PM2.5 predictions.

## Conclusion
The hybrid CNN-LSTM model effectively predicted PM2.5 concentrations in Sri Lankan urban cities, demonstrating high accuracy and reliability compared to standalone models. The model's architecture shows promise for extending predictive capabilities using satellite imagery and advanced deep learning techniques.

## Future Directions:
- Enhance model generalization with additional data (meteorological, traffic, land use).  
- Explore advanced architectures (Transformers, Graph Neural Networks).  
- Deploy a **real-time air quality monitoring system** with public dashboards.  
- Extend methodology to regions lacking dense sensor networks by leveraging satellite-only predictions.


## Contributing
Contributions are welcome! Please submit bug reports or feature requests via the GitHub issue tracker.


## Acknowledgments
We would like to express our heartfelt gratitude to our supervisor, Dr. Nalin Harischandra from the Faculty of Engineering, University of Peradeniya, for his invaluable 
guidance, support, and mentorship, which enabled us to complete this project related to the courses EE 405 – Undergraduate Project I & EE 406 – Undergraduate Project II on time throughout the process.

## Contact Information
For questions or inquiries, please contact our team,
- [Lahiru Herath](mailto:e18132@eng.pdn.ac.lk)
- [Ishan Bhanuka](https://github.com/IshanBhanuka)
- [Kaushan Nanayakkara](mailto:e18216@eng.pdn.ac.lk)

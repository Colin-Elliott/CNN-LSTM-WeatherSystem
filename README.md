# Multi-dimensional Weather Prediction System (CNN-LSTM)

## Project Overview
This project implements a hybrid CNN-LSTM model for multi-task meteorological forecasting using a 10-day sliding window approach. The system is designed to predict multiple weather parameters (temperature, humidity, pressure, wind) and classify weather types simultaneously.

## Dataset
The project uses weather data from Baoshan district in Shanghai, China, spanning from 2013 to 2017. The dataset is available in the `Weather-Baoshan(Shanghai).xlsx` file.

## Model Architecture
The hybrid model combines:
- **1D-CNN**: Feature extraction from weather parameters
- **Stacked LSTM**: Temporal modeling for time-series forecasting
- **Multi-task Framework**: Simultaneous prediction of multiple weather parameters and weather type classification

## Project Structure
- `LSTM-CNN.ipynb`: Implementation of the hybrid CNN-LSTM model
- `LSTM.ipynb`: Implementation of the LSTM baseline model
- `CNN.ipynb`: Implementation of the CNN baseline model
- `MLP.ipynb`: Implementation of the MLP baseline model
- `Weather-Baoshan(Shanghai).xlsx`: Weather dataset from Baoshan district, Shanghai (2013-2017)

## Performance
The hybrid CNN-LSTM model achieved significant improvements over baseline models:
- **Test MSE**: 0.005
- **Error Reduction**: 66.7% compared to LSTM baseline (0.015)
- **Error Reduction**: 58.3% compared to CNN baseline (0.012)

## Methodology
1. **Data Preprocessing**:
   - Data cleaning
   - Normalization
   - Time-series generation with 10-day sliding window

2. **Model Development**:
   - Feature extraction using 1D-CNN
   - Temporal modeling with stacked LSTM
   - Multi-task learning framework implementation

3. **Model Evaluation**:
   - Hyperparameter tuning
   - Benchmarking against LSTM, CNN, and MLP baselines
   - Performance evaluation using Mean Squared Error (MSE)

## Requirements
- Python 3.x
- TensorFlow/Keras
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Usage
1. Open the desired notebook (e.g., `LSTM-CNN.ipynb`) in Jupyter Notebook
2. Run the cells sequentially to:
   - Load and preprocess the data
   - Build and train the model
   - Evaluate model performance
   - Visualize results

## Contributors
- Project Lead: [Colin Elliott]
- Team Members: [Zhi Yang], [Huanan Liu]

## License
This is an academic course project. All rights reserved.
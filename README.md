# Amazon-Stock-Prediction-using-CNN-LSTM-model

This project focuses on predicting Amazon's closing stock prices using historical data from 2000 to 2024. The goal was to develop a robust deep learning model that captures market patterns and delivers accurate predictions.

We implemented a hybrid CNN + LSTM architecture to leverage both spatial feature extraction (via CNN) and temporal sequence learning (via LSTM).

🔍 Key Highlights:

Data Source: Amazon stock prices (2000–2024)
Model Architecture: Convolutional Neural Network (CNN) + Long Short-Term Memory (LSTM)
Batch Sizes Tested: 64, 128, and 256

Observation: A noticeable decline in variance capture (R-squared score) was observed as batch size increased, indicating reduced predictive accuracy.
Time Lags Tested: 50, 80, and 100 previous time steps were used to predict future prices (51st, 81st, 101st respectively).

Insight: Similar to batch size, increasing time lag also led to a decrease in R-squared, suggesting a limit to how much historical context enhances prediction.

📊 Performance Metric:

R-squared (Coefficient of Determination) was used to evaluate model performance, with the highest R-squared value reaching 99.76% under optimal configurations.

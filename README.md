# Carbon Emission Forecasting using LSTM

This repository presents a comprehensive approach to forecasting carbon emissions using advanced LSTM (Long Short-Term Memory) neural networks. As climate change and environmental sustainability become increasingly critical, accurate forecasting of carbon emissions is essential for policymakers, researchers, and industries aiming to mitigate environmental impacts. This project harnesses deep learning techniques to analyze historical carbon emission trends and predict future values with high accuracy. By leveraging sequential data modeling capabilities of LSTMs, the project offers valuable insights for strategic environmental planning and decision-making.

## Project Structure

- **carbon_emissions.csv**: Input dataset containing historical carbon emissions data.
- **carbon_emission_forecasting_lstm.py**: Python script to preprocess data, build, train, and evaluate the LSTM model.
- **Carbon_Emissions_Forecast.xlsx**: Output Excel file containing both historical and forecasted emissions data.

## Requirements

- Python 3.x
- TensorFlow
- Pandas
- Numpy
- Scikit-learn
- Matplotlib

Install dependencies:
```bash
pip install tensorflow pandas numpy scikit-learn matplotlib
```

## Usage

1. Prepare your dataset `carbon_emissions.csv` with the following structure:

```
Year,CO2_Emissions
1990,3000
1991,3050
...
```

2. Run the script:
```bash
python carbon_emission_forecasting_lstm.py
```

3. The script will:
   - Normalize the data.
   - Create sequences for the LSTM model.
   - Train the model on the training dataset.
   - Predict on the test dataset.
   - Forecast future carbon emissions.
   - Export the results to `Carbon_Emissions_Forecast.xlsx`.

4. Visualizations:
   - Actual vs Predicted Emissions
   - Forecasted Future Emissions

## Model Details

- 2 LSTM layers with 50 units each
- Dense layer with 1 output unit
- Adam optimizer
- Mean Squared Error (MSE) loss function
- Normalization using MinMaxScaler
- Window size (time_step) of 5 years

## Output

- Training and Test RMSE (Root Mean Squared Error)
- Graphs comparing actual and predicted emissions
- Forecasted emissions for the next 10 years
- Excel file with historical and forecasted data

## Author

Ayebawanaemi Geraldine Winston


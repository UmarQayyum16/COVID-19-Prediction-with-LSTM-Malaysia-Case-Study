# COVID-19-Prediction-with-LSTM-Malaysia-Case-Study

## Introduction

The year 2020 marked a global pandemic with the spread of COVID-19. This project aims to leverage deep learning, specifically LSTM (Long Short-Term Memory) neural networks, to predict daily new COVID-19 cases in Malaysia. The prediction models consider two scenarios: single-step and multi-step windows. The features include the columns: cases_new, cases_import, cases_recovered, and cases_active.

## Data Source

The dataset used for this project is sourced from the [MoH-Malaysia/covid19-public](https://github.com/MoH-Malaysia/covid19-public) repository, providing official data on the COVID-19 epidemic in Malaysia.

## Project Workflow

1. **Data Loading and Inspection:**
   - Load the COVID-19 dataset from [MoH-Malaysia/covid19-public](https://github.com/MoH-Malaysia/covid19-public).
   - Inspect and visualize the data to understand its structure and distribution.

2. **Data Cleaning and Preprocessing:**
   - Handle missing values and outliers.
   - Convert data types and format date columns.
   - Normalize the data for better model training.

3. **Exploratory Data Analysis (EDA):**
   - Explore the distribution of key features.
   - Visualize trends and patterns in COVID-19 cases.
   - Identify any correlations between features.

4. **Data Windowing:**
   - Create windowed datasets for both single-step and multi-step scenarios.

5. **Model Development:**
   - Design LSTM neural network models for both scenarios.
   - Train the models using the prepared windowed datasets.
   - Utilize TensorFlow and Keras for model implementation.

6. **Model Evaluation:**
   - Evaluate the models on the validation and test datasets.
   - Calculate Mean Absolute Percentage Error (MAPE) for performance assessment.

7. **TensorBoard Monitoring:**
   - Utilize TensorBoard to monitor training loss.
   - Ensure the convergence and stability of the models during training.

8. **Results and Visualization:**
   - Save the trained models.
   - Generate plots for training loss and model performance.
   - Include a graph comparing predicted and actual COVID-19 cases.

## Architecture

### Single-Step Model Architecture
   ![model_1_architecture](https://github.com/UmarQayyum16/COVID-19-Prediction-with-LSTM-Malaysia-Case-Study/assets/149918632/edf0c85c-6a63-495b-8ab0-1542a774ffa7)


### Multi-Step Model Architecture
   ![model_2_architecture](https://github.com/UmarQayyum16/COVID-19-Prediction-with-LSTM-Malaysia-Case-Study/assets/149918632/90328058-753a-457b-b50b-16c775d47007)

## Predicted vs. Actual COVID-19 Cases

### Single-Step Scenario

   ![single_step_result](https://github.com/UmarQayyum16/COVID-19-Prediction-with-LSTM-Malaysia-Case-Study/assets/149918632/d77db4f8-3d64-487c-8b82-6d91e88029f2)


In the graph above, the blue line represents the actual daily new COVID-19 cases, while the orange line indicates the predictions made by the single-step LSTM model. The close alignment between the two lines demonstrates the model's accurate predictions.

### Multi-Step Scenario

   ![multi_step_result](https://github.com/UmarQayyum16/COVID-19-Prediction-with-LSTM-Malaysia-Case-Study/assets/149918632/cca80ae5-cb66-4a88-8735-d6d749edb7c7)


For the multi-step scenario, the blue line represents the actual cases, and the orange line depicts the predictions made by the multi-step LSTM model. The model effectively captures the trend, providing accurate forecasts for the next 30 days.

These visualizations showcase the effectiveness of the LSTM models in predicting COVID-19 cases in both single and multi-step scenarios.

## Model Performance

### Single-Step Model Performance
- Validation MAPE: 0.01%
- Test MAPE: 0.03%

### Multi-Step Model Performance
- Validation MAPE: 0.01%
- Test MAPE: 0.03%

## Credits
The dataset used in this project is sourced from [MoH-Malaysia/covid19-public](https://github.com/MoH-Malaysia/covid19-public). We appreciate their efforts in providing official data on the COVID-19 epidemic in Malaysia.


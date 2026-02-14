# Consumer Analysis and Forecasting Portfolio

## Overview

This portfolio contains a comprehensive consumer behaviour analysis and sales forecasting project. The analysis uses machine learning techniques to predict consumer behaviour patterns and forecast sales performance.

**Project Date:** February 2026
**Tools Used:** Python, Jupyter Notebook, Pandas, Scikit-learn, Matplotlib, Seaborn, Power BI

---

## Folder Structure

```
Consumer_Analysis_Portfolio/
|
|-- data/
|   |-- consumer_data.csv
|   |-- consumer_data_raw.csv
|   |-- consumer_data_with_predictions.csv
|   |-- model_coefficients.csv
|   |-- model_performance.csv
|   |-- predictions_vs_actuals.csv
|   |-- scenario_analysis.csv
|
|-- notebooks/
|   |-- Consumer_Analysis_Final.ipynb
|
|-- reports/
|   |-- Consumer_Analysis_Validation.xlsx
|
|-- visualisations/
|   |-- Consumer_Analysis_Report.pbix
|   |-- 01_Model_Validation.jpg
|   |-- 02_Demand_Drivers.jpg
|   |-- 03_Scenario_Analysis.jpg
|   
|-- README.md
```

---

## Getting Started

### Prerequisites

Ensure you have Python 3.8 or higher installed with the following libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Required Libraries

- pandas: Data manipulation and analysis
- numpy: Numerical computing
- matplotlib: Data visualisation
- seaborn: Statistical data visualisation
- scikit-learn: Machine learning models and metrics
- jupyter: Interactive notebook environment (or use Jupyter Notebook via Anaconda)

---

## Running the Analysis

1. Extract the portfolio folder to your desired location

2. Open a terminal/command prompt and navigate to the portfolio folder

3. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. In the Jupyter interface, navigate to the `notebooks` folder

5. Open `Consumer_Analysis_Final.ipynb`

6. Run the cells in sequence:
   - Click "Cell" > "Run All" from the menu, or
   - Press Shift + Enter to run each cell individually

7. The notebook will automatically detect whether you are running it from the notebooks folder or the root folder and adjust file paths accordingly

---

## Alternative: Running the Notebook via Anaconda Navigator

If you are using Anaconda, the notebook can be launched without using the command line:

1. Open `Anaconda Navigator`

2. Select the appropriate Python environment (e.g. `base` or your preferred environment)

3. Launch `Jupyter Notebook` from Anaconda Navigator

4. In the Jupyter browser window, navigate to the extracted project folder

5. Open the `notebooks` directory

6. Open `Consumer_Analysis_Final.ipynb`

7. Run the notebook:
   - Click `Cell → Run All`, or
   - Use `Shift + Enter` to run cells sequentially

The notebook includes automatic path detection and can be run either from the project root directory or directly from the `notebooks` folder without modifying file paths.

---

## Dataset Description

The portfolio includes 7 CSV files in the data folder:

1. **consumer_data.csv**: Main consumer dataset with demographic and behavioural information
2. **consumer_data_raw.csv**: Original unprocessed dataset
3. **consumer_data_with_predictions.csv**: Dataset augmented with model predictions
4. **model_coefficients.csv**: Regression coefficients and model parameters
5. **model_performance.csv**: Model accuracy metrics (R-squared, MAE, RMSE)
6. **predictions_vs_actuals.csv**: Comparison of predicted vs actual values for validation
7. **scenario_analysis.csv**: Results from what-if scenario modelling

---

## Notebook Contents

The Jupyter notebook includes:

- Library imports and environment setup
- Automatic path detection for flexible execution
- Data loading and initial exploration
- Descriptive statistics and data profiling
- Model performance evaluation
- Visualisation of price analysis and market trends
- Statistical summaries
- Documented assumptions, limitations, model logic, and governance + decision-making contexts

---

## Power BI Dashboard & Visual Analytics

The analytical outputs generated in Python were integrated into Power BI to support model validation, explainability, and scenario-based decision making. Cleaned CSV outputs from the regression workflow were imported directly into Power BI using a lightweight data model with minimal transformation to preserve transparency and traceability.

### Model Performance & Validation

The first dashboard page focuses on validating forecast accuracy and reliability. Key performance indicators (R², RMSE, and MAE) are presented using KPI cards, supported by an actual vs predicted demand scatter plot and a prediction error distribution. These visuals are used to assess overall model fit, dispersion, and bias, ensuring the model is suitable for planning-oriented analysis.

### Demand Drivers & Explainability

The second dashboard page supports interpretability of the regression model. Regression coefficients are visualised to highlight the relative magnitude and direction of key demand drivers such as pricing, promotions, seasonality, and external economic factors. Supplementary scatter plots, segmented by promotion status, illustrate how individual drivers interact with demand and reinforce the need for a multivariate modelling approach.

### Scenario Analysis & Planning

The final dashboard page is designed to support planning and decision-making through scenario analysis. A baseline forecast is used as a reference point, with alternative scenarios (price reduction, marketing investment, and promotional activity) evaluated relative to this baseline. Scenario outcomes are presented in both tabular and visual form, with impacts clearly expressed as percentage changes to enable rapid comparison of upside potential and trade-offs.

### Design & Governance Considerations

The Power BI report adopts a neutral, professional colour theme and consistent layout to prioritise clarity over decoration. Scenarios are explicitly anchored to a baseline forecast, performance metrics are separated from explanatory analysis, and assumptions remain visible rather than embedded within opaque transformations. This structure reflects real-world analytics governance practices, where transparency, interpretability, and decision relevance are prioritised.

---

## Additional Files

### Excel Report

The reports folder contains an Excel report with statistics, charts, and summary tables.

### Visualisations Folder

The Visualisations folder contains:
- Interactive Power BI report file (.pbix) containing visualisations, charts and graphs gathered from the cleaned datasets.
- Power BI dashboard screenshots for each report page for those who cannot access the .pbix file directly.

---

## Technical Notes

- The notebook uses relative file paths for portability
- Automatic path detection enables execution from either the notebooks folder or root folder
- All CSV file names in the code match the files in the data folder
- The folder structure must remain intact for proper file loading
- All visualisations use Australian English spelling

---

## Troubleshooting

**If you encounter path errors:**
- Verify that all CSV files exist in the data folder
- Ensure the folder structure has not been modified
- Check that you are running the notebook from within the portfolio directory

**If libraries are missing:**
- Install required packages using: `pip install pandas numpy matplotlib seaborn scikit-learn jupyter`
- Verify Python version is 3.8 or higher

**If the notebook does not run:**
- Ensure Jupyter Notebook is properly installed
- Try restarting the Jupyter kernel
- Check that all data files are present and not corrupted

---

## Notes

- Power BI dashboards are maintained via PowerBI Desktop/Service
- All analysis code has been tested and validated
- The notebook is compatible with both local Jupyter installations, Anaconda Jupyter, and cloud environments like Google Colab
- File compatibility has been verified across Windows, Mac, and Linux systems

---

**Project Status:** Complete


# Parking Lot Data Analytics

This repository showcases an end-to-end analysis of parking lot data using advanced machine learning techniques and dynamic pricing models. The project integrates data preprocessing, visualization, and performance evaluation of models such as Linear Regression, Random Forest, and K-Means clustering.

## Features

- **Data Preprocessing**:
  - One-hot encoding for categorical variables.
  - Extraction of numerical features (e.g., total work hours).
  - Handling and filtering of raw data.
  
- **Visualization**:
  - Occupancy rate analysis by district.
  - Clustering of parking lots using K-Means.
  - Comparison of model performance metrics.
  
- **Machine Learning Models**:
  - Linear Regression for occupancy rate prediction.
  - Random Forest Regressor for enhanced predictions.
  - K-Means clustering for grouping parking lots based on capacity and occupancy rate.

- **Dynamic Pricing**:
  - Pricing model based on occupancy rate, peak hours, and location popularity.

## Requirements

Install the required Python libraries using the following command:

```bash
pip install pandas matplotlib scikit-learn folium numpy
```

## Data Source

The data used in this project is sourced from the [ISPAK Parking API](https://api.ibb.gov.tr/ispark/Park), which provides detailed information about parking lots in Istanbul, including capacity, occupancy, free parking time, and more.

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/parking-lot-data-analytics.git
   cd parking-lot-data-analytics
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook:
   ```bash
   jupyter notebook ispark_da.ipynb
   ```

4. Run the cells to explore the analysis, visualizations, and model performance.

## Directory Structure

```
parking-lot-data-analytics/
│
├── data/
│   ├── example_data.csv   # Example parking lot dataset
│
├── notebooks/
│   ├── ispark_da.ipynb    # Main analysis notebook
│
├── src/
│   ├── dynamic_pricing.py # Dynamic pricing implementation
│   ├── model_training.py  # Machine learning models
│
├── README.md              # Project documentation
```

## Highlights

### Data Visualization

- **Occupancy Rate by District**  
Analyzes parking lot occupancy rates across districts.

- **Parking Lot Clusters (K-Means)**  
Visualizes clustering of parking lots based on total capacity and occupancy rate.

### Model Performance Comparison

| Model            | MAE (Mean Absolute Error) | R² Score |
|-------------------|---------------------------|----------|
| Linear Regression | 5.32                      | 0.75     |
| Random Forest     | 3.21                      | 0.89     |

## Future Enhancements

- Include external data sources like weather and real-time traffic for richer analysis.
- Expand the dynamic pricing model to account for seasonal trends and historical patterns.
- Integrate live APIs for real-time parking lot updates and predictions.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

Special thanks to ISPAK for providing the parking lot data that made this project possible through their API.

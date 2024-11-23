# Data Analysis and Regression Modeling

This repository provides a Python implementation for loading, exploring, visualizing, preprocessing, and modeling data using regression techniques. The project uses libraries like `pandas`, `matplotlib`, `seaborn`, and `scikit-learn` to handle and analyze the dataset.

## Features

- **Data Loading and Exploration**: Loads a dataset, provides an overview, checks for missing values, and prints dataset information.
- **Data Visualization**: Generates histograms, bar plots, and pair plots for insights into features and relationships.
- **Data Preprocessing**: Cleans data, encodes categorical features, and splits the dataset into training and testing sets.
- **Model Training**: Trains multiple regression models including Linear Regression, Lasso, and Ridge.
- **Hyperparameter Tuning**: Performs grid search to optimize Ridge regression.
- **Model Evaluation**: Evaluates models using metrics like R², Mean Absolute Error, and Mean Squared Error.

## Requirements

The following Python libraries are required:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Install the dependencies using the following command:

```bash
pip install -r requirements.txt
```

> **Note**: Ensure you have Python 3.7 or later installed.

## File Structure

- `main.py`: Contains the core implementation.
- `January_MyCall_2022.csv`: Placeholder for the dataset (update with the actual file).
- `README.md`: Documentation for the project.

## Usage

1. **Clone the repository**:
   ```bash
   https://github.com/MohamadPirniakan/Customer-Call-Quality-Analysis.git
   cd your-repo-name
   ```

2. **Run the script**:
   Update the `filepath` variable in `main.py` with the path to your dataset, then execute:

   ```bash
   python main.py
   ```

3. **Analyze the results**:
   Review the printed metrics, visualizations, and sample predictions for insights.

## Code Workflow

1. **Load Data**:
   ```python
   df = load_data(filepath)
   ```

2. **Visualize Data**:
   ```python
   visualize_data(df)
   ```

3. **Preprocess Data**:
   ```python
   X_train, X_test, y_train, y_test = preprocess_data(df)
   ```

4. **Train Models**:
   ```python
   results = train_models(X_train, y_train)
   ```

5. **Hyperparameter Tuning**:
   ```python
   best_model = grid_search_ridge(X_train, y_train)
   ```

6. **Evaluate Best Model**:
   ```python
   evaluate_model(best_model, X_test, y_test)
   ```

## Visualizations

The script generates the following plots:

- Histograms for categorical features.
- Bar plots showing the average rating by categorical features.
- Pair plots for latitude and longitude with rating distribution.
- Scatter plot comparing true vs. predicted ratings.

## Sample Data

The dataset (`January_MyCall_2022.csv`) is expected to have the following columns:

- `operator`
- `inout_travelling`
- `network_type`
- `rating`
- `calldrop_category`
- `state_name`
- `latitude`
- `longitude`

Replace the placeholder file path with your actual dataset location.

## Acknowledgments

This project uses `scikit-learn` for machine learning and `matplotlib`/`seaborn` for data visualization.

---

Feel free to contribute, raise issues, or suggest improvements. 😄
```

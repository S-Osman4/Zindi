# Wildfire Prediction Challenge

![Project Status](https://img.shields.io/badge/status-active-brightgreen)
![Python Version](https://img.shields.io/badge/python-blue)
![License](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributors](#contributors)
- [License](#license)

## Introduction

This repository contains the code and analysis for the [**Zindi Wildfire Prediction Challenge**](https://zindi.africa/competitions/predict-fire-extent/data). The goal of the project was to predict the burned area of wildfires in Zimbabwe from 2014 to 2016 using machine learning models.

This challenge was beginner-friendly and provided a supportive environment for newcomers to learn and grow in the field of machine learning.

## Dataset

The dataset provided by Zindi includes:

- **Train Dataset**: `data/Train.csv` - Contains historical wildfire data including the target variable `burn_area`.
- **Test Dataset**: `data/Test.csv` - Contains the same features as the train dataset but without the target variable.
- **Variable Definition** : `data/variable_definitions.csv` - Contains description the variables found in train and test datasets.

### Additional Information

- **Climate Data**: Derived from TerraClimate, containing various climate-related variables.
- **Land Cover Data**: Land cover type percentages for the areas.
- **Population Density**: UN-Adjusted Population Density estimates.
- **Elevation**: Mean elevation in meters.
- **Monthly Precipitation**: Estimates derived from TRMM.

## Project Structure


## Installation

To set up the project locally, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/S-Osman4/Zindi.git
    cd Zindi/Wildfire\ Prediction\ Challenge
    ```

2. Install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

3. Launch the Jupyter Notebook:

    ```bash
    jupyter notebook notebooks/Wildfire_Prediction_Challenge.ipynb
    ```

## Usage

Open the `Wildfire_Prediction_Challenge.ipynb` notebook to follow along with the analysis. The notebook includes:

1. **Data Preprocessing**: Cleaning and preparing the data for modeling.
2. **Model Training**: Training various models including Random Forest, Gradient Boosting, XGBoost, and LightGBM.
3. **Evaluation**: Comparing model performance using metrics such as RMSE.

## Results

The evaluation metric for this competition was Root Mean Squared Error (RMSE). The model was trained on the provided data and evaluated on the test set with the following results:

- **Public Score**: `0.019948181`
- **Private Score**: `0.018610606`

The project was developed using the Google Colab environment.

## Contributors

- [Shamso Osman](https://github.com/S-Osman4)

## License

This project is licensed under the CC-BY-SA 4.0 License - see the [LICENSE](LICENSE) file for details.




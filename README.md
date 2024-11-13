# Data Analysis of Listings Dataset

This project performs a comprehensive analysis of a dataset containing listings information. The analysis includes data loading, exploration, and visualization of key statistics and insights.

## Table of Contents

- [Project Overview](#project-overview)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Functions](#functions)
- [License](#license)

## Project Overview

The main goal of this project is to analyze a CSV file (`listings.csv`) containing various listings data. The analysis includes:

- Loading the dataset and handling potential errors.
- Displaying key statistics and information about the dataset.
- Visualizing the distribution of numerical features through histograms.

## Requirements

To run this project, you need the following Python libraries:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `tabulate`

You can install these libraries using pip:

```bash
pip install numpy pandas matplotlib seaborn tabulate

Installation
- Clone the repository or download the project files to your local machine.
- Ensure that you have the required libraries installed (as mentioned above).
- Place the listings.csv file in the same directory as the script.

Functions
The script contains the following key functions:

load_data(file_path): Loads the CSV file and handles errors related to file access and parsing.
display_data_info(df): Analyzes the dataset and prints various statistics, including:
Number of rows and columns
Missing data information
Data types of each column
Summary statistics for numerical and categorical data
Correlation matrix for numerical columns
Value counts for categorical columns
plot_numerical_histograms(df): Plots histograms for all numerical columns in the dataset.
License
This project is licensed under the MIT License. See the LICENSE file for more information.
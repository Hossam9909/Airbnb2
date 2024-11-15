Airbnb Price Analysis
Project Overview
This project explores the factors influencing Airbnb listing prices using data analysis and machine learning techniques. By following the CRISP-DM process, the project answers key business questions and provides actionable insights for hosts and stakeholders in the Airbnb ecosystem.

Business Questions
The analysis aims to answer the following questions:

What factors influence the price of an Airbnb listing?
How does availability correlate with the number of reviews or price?
Are there location-based trends in reviews, pricing, or popularity?
How does the room type affect the average price and availability of listings?
Do listings with more frequent reviews tend to have higher ratings or lower availability?
Dataset
The dataset contains information on Airbnb listings, including:

Listing Details: Room type, price, availability, and minimum nights.
Host Details: Host name, number of listings.
Location: Neighborhood and geographic coordinates.
Reviews: Number of reviews, last review date, and reviews per month.
Preprocessing Steps
Handling Missing Data:

Columns with 100% missing values were removed.

Imputation Considerations:

Median Imputation for 'reviews_per_month': Given that the median is lower than the mean, using the median (1.45) for imputation would be a good choice. This approach is robust to outliers and will provide a more representative value for listings with missing data.

using a placeholder like "No reviews" for missing values in the last_review column . This clearly indicates that there are no reviews available for those listings.

filling the missing values in the price column with the median (104.0) is likely the best approach. It balances the need to provide a reasonable estimate without introducing the bias that could come from using the mean or zero.


Feature Engineering:

Converted categorical variables into dummy variables.
Extracted meaningful insights from review-related data.
Analysis and Modeling
Methodology
Exploratory Data Analysis (EDA):

Visualized distributions of numerical columns.
Assessed relationships between features (e.g., correlations).
Identified trends across neighborhoods and room types.
Regression Modeling:

A linear regression model was used to predict Airbnb prices based on features like room type, location, and availability.
The model was evaluated using:
R-squared: Proportion of variance explained.
Mean Squared Error (MSE): Average squared difference between actual and predicted prices.
Cross-Validation: Ensured robustness of the model.
Key Findings
Room type significantly impacts listing prices, with "Entire home/apt" commanding higher rates.
Listings with frequent reviews tend to have higher prices, reflecting demand and popularity.
Geographic location correlates with pricing patterns, with central neighborhoods being more expensive.
Results
The project successfully answered the business questions and identified actionable insights for Airbnb hosts:

Price optimization strategies based on room type and location.
Importance of reviews in driving demand and pricing decisions.
Data-driven recommendations for availability and minimum stay settings.

Repository Structure

├── data/                     # Dataset used for the project
├── notebooks/                # Jupyter Notebooks with code and analysis
│   ├── exploratory_analysis.ipynb
│   ├── modeling_and_results.ipynb
├── README.md                 # Project overview and results
├── requirements.txt          # List of required libraries

How to Run
Clone the repository:
git clone https://github.com/username/airbnb-price-analysis.git

Install the required libraries:
pip install -r requirements.txt

Open the Jupyter Notebooks in the notebooks/ folder to explore the analysis and results:
exploratory_analysis.ipynb: Data exploration and visualization.
modeling_and_results.ipynb: Machine learning pipeline and results.
Libraries Used
Pandas: Data manipulation and preprocessing.
NumPy: Numerical operations.
Matplotlib/Seaborn: Data visualization.
Scikit-learn: Machine learning and model evaluation.
Tabulate: Cleanly displaying tabular data.
Acknowledgments
This project was inspired by publicly available Airbnb data and aims to provide insights for better decision-making. Special thanks to the data providers and the open-source community.





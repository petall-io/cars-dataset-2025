# Cars Dataset Analysis (2025)

## Overview
Analyze global car production and pricing trends by region, fuel type, and performance characteristics, with a focus on comparing electric vehicles to internal combustion engine vehicles.

## Objective
Apply data cleaning, transformation, and analysis techniques to explore global car production, pricing, and performance differences across regions and fuel types.

## Dataset
- Source: https://www.kaggle.com/datasets/abdulmalik1518/cars-datasets-2025
- Size: 1,218 rows, 11 columns (raw)
- Accessed: August 5, 2025

## Tools
- Python (pandas, numpy)
- Tableau Public

## Data Processing and Feature Engineering
1. Data cleaning and normalization (missing values, duplicates, column renaming)
2. Use regular expressions to identify and separate engine and battery capacities
3. Expand rows with multiple engines and capacities and create a separate index to identify variants
4. Normalize numeric columns and address ranges by creating 'min' and 'max' columns
5. Standardize fuel types and car brands, and map car brands to regions and countries
6. Assign price tiers based on price bins and create new columns for region, country, and price tier
7. Export cleaned dataset to Tableau Public for visualization and dashboard creation

## Key Insights
- Europe and Asia are comparable in car production, while North America produces less than half the production of Europe or Asia individually
- Europe has the most even spread of car production in all price tiers, prioritizing mostly Premium and Midrange vehicles, but also has respectable Budget, Luxury, and Supercar production
- Asia primarily focuses on Budget and Midrange car production and some Premium cars, but minimal Luxury and Supercar production
- North America primarily focuses on Midrange and Premium car production, and has minimal car production in the other price tiers
- Aside from Supercars, Electric vehicles are the most expensive among the other fuel types, with the highest average horsepower and torque
- Electric vehicles fall behind Petrol and Hybrid cars in average total speed, despite having higher average horsepower and torque, likely due to thermal limitations and differences in sustained high-speed performance compared to ICE vehicles
- Diesel cars consistently cost the least while also having the lowest performance among fuel types

## Tableau Dashboard
🔗 [View on Tableau Public](https://public.tableau.com/views/CarsDataset2025Analysis/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Project Structure
### car_dataset_2025.ipynb
- my notebook, where you can read my code and further explanation on design choices and assumptions
### requirements.txt
- list of dependencies to replicate this analysis
### .gitignore
- files that I don't want to push to github (file size, potentially sensitive information, etc.)

## Reproducibility
This analysis was conducted in Python 3.11 using a virtual environment.  
To reproduce the analysis, create a virtual environment, install the dependencies listed in requirements.txt, and run the notebook from top to bottom.

## Assumptions and Limitations
- Analysis is limited to the cars represented in the dataset and may not reflect total global production.
- Performance metrics are based on listed specifications and do not account for real-world driving conditions.
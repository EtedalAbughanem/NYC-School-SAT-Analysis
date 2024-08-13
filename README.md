# NYC-School-SAT-Analysis
Exploratory data analysis on NYC schools, focusing on identifying schools with the best math results, top performers based on combined SAT scores, and the borough with the largest standard deviation in SAT scores.

## Project Overview

This project involves exploratory data analysis (EDA) on a dataset of NYC schools. The analysis aims to:

1. Identify schools with the best math results.
2. Determine the top 10 performing schools based on combined SAT scores.
3. Find the borough with the largest standard deviation in combined SAT scores.

## Dataset

The dataset used for this analysis is `schools.csv` and includes the following columns:

- `school_name`: Name of the school
- `borough`: Borough where the school is located
- `building_code`: Building code of the school
- `average_math`: Average math score
- `average_reading`: Average reading score
- `average_writing`: Average writing score
- `percent_tested`: Percentage of students tested

## Analysis

1. **Best Math Results:**
   - Filter schools with an average math score of at least 80% of the maximum possible score (800).
   - Save the results in a DataFrame named `best_math_schools`, sorted by `average_math` in descending order.

2. **Top 10 Performing Schools Based on Combined SAT Scores:**
   - Calculate the total SAT score by summing `average_math`, `average_reading`, and `average_writing`.
   - Save the top 10 performing schools in a DataFrame named `top_10_schools`, including `school_name` and `total_SAT`.

3. **Borough with the Largest Standard Deviation in Combined SAT Scores:**
   - Calculate the count, mean, and standard deviation of `total_SAT` scores for each borough.
   - Identify the borough with the largest standard deviation and save the results in a DataFrame named `largest_std_dev`.
   - The DataFrame contains columns: `borough`, `num_schools`, `average_SAT`, and `std_SAT`.

## Results

- **Best Math Schools:**
  Schools with the highest average math scores.

- **Top 10 Performing Schools:**
  Schools with the highest combined SAT scores.

- **Borough with Largest Standard Deviation:**
  The borough with the highest variation in SAT scores.

## Usage

To replicate the analysis, follow these steps:

1. Ensure you have the necessary library (`pandas`) installed.
2. Load the dataset into a pandas DataFrame.
3. Run the provided Python script to perform the analysis and generate results.

## Dependencies

- pandas


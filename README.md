# Optimization of Waste Transportation and Portfolio Management

## Overview
This repository contains the code and analysis for two major optimization problems addressed in Module 6 of the course. The first problem focuses on minimizing transportation costs for chemical waste disposal. The second problem involves optimizing an investor’s portfolio allocation to minimize risk while maximizing returns. The project is split into two parts:

1. **Waste Transportation Optimization**: The goal is to minimize the transportation cost of moving chemically processed waste from various facilities to disposal sites. Two approaches are compared: direct transportation and transportation via intermediate storage points.
2. **Portfolio Optimization**: The objective is to determine the optimal allocation of $1,000,000 into a set of six selected assets to minimize risk while maintaining expected returns.

## Project Structure
- **Waste Transportation Optimization**:
  - `waste_transportation.R`: Code for calculating transportation costs using two methods (direct transportation vs. intermediate storage).
  - `waste_transportation_analysis.xlsx`: Contains the data tables with waste transportation costs and storage limits for both methods.

- **Portfolio Optimization**:
  - `portfolio_optimization.R`: Code for optimizing the portfolio allocation using an investor’s selected assets and minimizing risk based on different expected return thresholds.
  - `portfolio_data.csv`: Contains the assets' expected returns and the covariance matrix between the assets.
  - `portfolio_analysis.xlsx`: Spreadsheet showing various portfolio allocations and risk analysis for different return rates.

## Getting Started
To run the scripts, you will need to have R installed along with the following packages:
- `ggplot2`
- `dplyr`
- `quadprog`
- `readr`

You can install the necessary packages with the following R command:
```r
install.packages(c("ggplot2", "dplyr", "quadprog", "readr"))
```

## How to Run
### Part 1: Waste Transportation Optimization
1. Run `waste_transportation.R` to calculate the transportation costs for both the direct route and the intermediate storage route.
2. The results of the transportation costs will be displayed in the console, and the most economical transportation method will be selected based on the lowest cost.

### Part 2: Portfolio Optimization
1. Run `portfolio_optimization.R` to perform portfolio optimization and determine the optimal allocation of funds across the six assets.
2. The script will generate a table showing the optimal investment amounts for minimizing risk at various expected return levels.
3. A graph will be generated that shows the relationship between minimized risk and expected portfolio return.

## Key Results
### Part 1: Waste Transportation Optimization
- **Direct Transportation**: Total cost = $3425
- **Intermediate Storage**: Total cost = $2050
- **Conclusion**: The second method (using intermediate storage) is the most cost-effective option for transporting waste.

### Part 2: Portfolio Optimization
- The optimal allocation of $1,000,000 is:
  - **Bonds**: $824,801.13
  - **Call Options**: $3,987.21
- **Conclusion**: The portfolio optimization minimizes risk while maintaining expected returns. A graph shows the relationship between minimized risk and portfolio return, with minimized risk staying consistent at lower return rates and increasing at higher return rates.

## Conclusion
This repository demonstrates the application of optimization techniques for two different real-world problems: reducing transportation costs for waste disposal and minimizing risk in portfolio investment. The methods and results presented here can be applied to similar scenarios in logistics and finance for cost minimization and risk management.

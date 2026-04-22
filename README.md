# Movie Correlation Analysis in Python

![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)
![Jupyter Notebooks](https://img.shields.io/badge/jupyter_notebooks-ff7143.svg?style=for-the-badge&logo=Jupyter-Notebooks&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/matplotlib-%2345818e.svg?style=for-the-badge&logo=matplotlib&logoColor=white)
![Windows Terminal](https://img.shields.io/badge/Windows%20Terminal-%234D4D4D.svg?style=for-the-badge&logo=windows-terminal&logoColor=white)
![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white)
![Seaborn](https://img.shields.io/badge/seaborn-%23531414.svg?style=for-the-badge&logo=seaborn&logoColor=white)


## Overview
This project explores a movie industry dataset to identify which factors like budget, votes, or production company have the strongest correlation with the gross revenue of a film. The analysis is conducted in Python using libraries such as Pandas, Seaborn, and Matplotlib to clean, visualize, and analyze the data.


## [Reports](https://github.com/gauravkamble-insights/Movie-Correlation-Analysis-in-Python/blob/main/report/Movie%20Correlation%20Analysis%20in%20Python.pdf)  



### Preview
*Initial visualization of Budget vs. Gross Earnings using Matplotlib*  
<img width="1002" height="703" alt="Scatter plot budget vs gross earning" src="https://github.com/gauravkamble-insights/Movie-Correlation-Analysis-in-Python/blob/main/assets/Scatter%20plot%20budget%20vs%20gross%20earning.png" />
  
*Regression plot showcasing the positive correlation between Budget and Gross*
<img width="1002" height="695" alt="seaborn" src="https://github.com/gauravkamble-insights/Movie-Correlation-Analysis-in-Python/blob/main/assets/seaborn.png" />



## Project Structure
The project is organized into a single Jupyter Notebook (.ipynb) that handles the end-to-end data pipeline from ingestion to final correlation analysis.

## Dataset Overview
The [dataset](https://www.kaggle.com/datasets/danielgrijalvas/movies), sourced from Kaggle, contains 15 columns for thousands of films, including:
- **Budget:** The production cost of the movie.
- **Gross:** Total revenue generated.
- **Votes:** Number of user votes on platforms like IMDb.
- **Company, Genre, Rating, Released, Runtime, etc.**

## Analysis
### 1. **Data Cleaning:**
- **Missing Data:** Identifies null values (e.g., 28% missing in Budget, 2% in Gross).
- **Data Type Standardization:** Converts float values to integers for cleaner presentation.
- **Year Correction:** Extracts the correct release year from the released date string to resolve mismatches in the original year column.
- **Duplicates:** Drops redundant entries to ensure data quality.
  
### 2. **Exploratory Data Analysis (EDA):**
- Utilizes Scatter Plots and Regression Plots (via Seaborn) to visually confirm initial hypotheses regarding budget and revenue.  

### 3. **Correlation Analysis:**
- **Pearson Method:** Uses the default Pearson correlation to measure linear relationships between numeric variables.
- **Categorical Encoding ("Numerization"):** Converts non-numeric columns like "Company" and "Genre" into numeric codes to include them in the full correlation matrix.
- **Heatmap Visualization:** Generates high-density heatmaps to identify strong vs. weak correlation pairs at a glance.

## Key Questions Explored
**1. High Correlation Hypotheses:** Does a higher budget directly result in higher gross earnings?  
**2. Categorical Influence:** Do specific production companies significantly impact a movie's financial success?  
**3. Variable Impact:** Which other movie features (like user votes or runtime) show significant correlation with revenue?  

## Summary of Findings
**Top Correlations:** The two variables with the highest correlation to gross revenue are Budget (0.75) and Votes (0.63).
**Company Impact:** Contrary to initial predictions, the production company has a very low correlation with total revenue.
**Strong Pairs:** Several features, such as "Year" and "Corrected Year," show a perfect 1.0 correlation, while other notable relationships exist between votes and budget.

*Summary of the highest correlation pairs found in the dataset*
<img width="917" height="703" alt="correlation matrix" src="https://github.com/gauravkamble-insights/Movie-Correlation-Analysis-in-Python/blob/main/assets/correlation%20matrix.png" />  

## Author
- <b>©2026 Gaurav Kamble.  
- <b>[LinkedIn](https://www.linkedin.com/in/gaurav-kamble/)</b>
- <b>[Tableau Public](https://public.tableau.com/app/profile/datagaurav/vizzes)</b>
- <b>[Kaggle](https://www.kaggle.com/justgk)</b>
- <b>[Email](mailto:gauravksse@gmail.com)</b>

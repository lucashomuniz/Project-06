# ✅ PROJECT-06

In this project, we will conduct a multivariate analysis to answer the question: **"Which factors most influence housing occupancy rates?"** The analysis is led by a technology company specialized in data and statistics, focusing on neighborhoods within a specific city to generate insights for various sectors.

The results can support both public and private decision-making. Local governments may use the findings to design more effective policies in areas like security and sanitation. Construction firms and investors can identify regions with higher growth and occupancy potential. The dataset includes demographic, economic, and environmental variables such as average number of rooms, building age, crime rate, pollution, distance to the city center, and residential taxes.

We will use **Python** and libraries like `pandas`, `numpy`, `scipy`, and `statsmodels` to perform hypothesis testing, regressions, and other statistical analyses. All work will be done in a Jupyter Notebook environment.Finally, key insights will be presented in an interactive **Power BI** dashboard, using **DAX** for creating analytical metrics—ensuring clear and actionable visualizations.

**Keywords**: Statistical Analysis, Business Analytics, Data Visualization, Python Language, Python Libraries, PowerBI, PowerQuery, DAX.

# ✅ PROCESS

We began the development with a detailed **Exploratory Data Analysis (EDA)** to understand the structure and distribution of the collected variables. In this phase, we used histograms and scatter plots to identify patterns and outliers. We observed that the dependent variable (**taxa_ocupacao**) had a slightly right-skewed distribution, indicating the possible presence of outliers. To reduce this distortion, we applied a logarithmic transformation, creating the variable **taxa_ocupacao_log**, which showed a distribution closer to normality, reducing skewness. Lastly, we also assessed the skewness of the other variables before proceeding with further analyses.

![Screenshot 2025-03-24 at 20 17 01](https://github.com/user-attachments/assets/cdcf10a1-ed05-4956-b912-0ea44857a74c)

In the next step, we performed a **Bivariate Analysis** to investigate the relationship between the dependent variable and each independent variable through a **correlation table**. We used the **Pearson correlation coefficient** to quantify the strength of linear relationships, identifying variables with greater predictive potential, such as the **average number of rooms per residence**, **crime rate**, and **distance to the city center**. This analysis was important as it allowed us to initially distinguish which variables were truly relevant to the target variable (occupancy rate) and which had little or no influence. Based on these results, we assessed the presence of **multicollinearity** among the independent variables using the **Variance Inflation Factor (VIF)**. This step enabled us to select only the most relevant and statistically reliable variables for the subsequent models.

![imagem2](https://github.com/user-attachments/assets/29952055-944f-4c7d-826e-350faebc9b23)

After identifying the need for data transformation, we also performed a **careful removal of outliers** using graphical analysis and statistical techniques, including the **Shapiro-Wilk Normality Test** and the **evaluation of skewness** for each variable. This step ensured that the following analyses would be conducted on more homogeneous and statistically robust data. With the dataset properly treated, we proceeded to build **Multiple Linear Regression Models**, developing five distinct versions, each incorporating improvements over the previous one:

> **Model 1 (Raw Data)**: Served as the baseline model to understand the overall behavior of the data without adjustments.

> **Model 2 (Standardized Data)**: Included data standardization techniques to improve the interpretation and comparability of coefficients.

> **Model 3 (Without Multicollinearity)**: Variables with high VIF were removed to mitigate the negative effects of multicollinearity.

> **Model 4 (Excluding low-significance variables – first optimization)**: Variables with high p-values, low statistical significance, were excluded.

> **Model 5 (Final optimization – only statistically relevant variables)**: A more rigorous selection process was applied, retaining only the most statistically significant variables.

![212121](https://github.com/user-attachments/assets/c68c8608-b7df-48e8-a072-52990ae461cc)

Each model was carefully evaluated using key metrics such as the **p-value**, essential for determining the significance of the variables, and the **R-Squared (R²) coefficient**, which indicates how much of the variability in housing occupancy the model is able to explain. Throughout the modeling process, we rigorously assessed the fundamental assumptions of multiple linear regression, including: **Linearity**, **Independence of errors**, **Homoscedasticity**, **Normality of residuals**, and **Absence of multicollinearity**. In the end, the fifth model, optimized after all adjustments, showed the best statistical performance, clearly identifying the factors that directly influence housing occupancy rates.

![Screenshot 2025-03-24 at 21 02 04](https://github.com/user-attachments/assets/174e3dab-8bf1-4e48-811f-d5f24fbc0cc9)

# ✅ CONCLUSION

In this project, we found that multicollinearity is a serious issue, as it can significantly compromise the quality and reliability of statistical models and introduce bias. To mitigate this risk, we applied the **Variance Inflation Factor (VIF)** to identify and remove highly correlated variables.

Through rigorous statistical analyses—including Pearson correlation, p-value evaluation, and multiple linear regressions—we clearly identified the most relevant factors influencing housing occupancy rates: `average number of rooms per residence`, `crime rate`, `presence of a river in the neighborhood`, `pollution rate`, `distance to the city center`, `teacher rate` and `homelessness rate`.

These variables are key determinants of housing occupancy and can support public decision-making in infrastructure and security planning, as well as guide private investors in strategic location assessments. Finally, based on the most relevant variables, we developed an interactive dashboard in Power BI, using PowerQuery for efficient data processing and DAX for building clear and objective metrics—delivering a robust analytical tool for strategic decision-making.

**Dashboard**:

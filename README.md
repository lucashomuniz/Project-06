# ✅ PROJECT-06

In this project, we will conduct a multivariate analysis to answer the question: **"Which factors most influence housing occupancy rates?"** The analysis is led by a technology company specialized in data and statistics, focusing on neighborhoods within a specific city to generate insights for various sectors.

The results can support both public and private decision-making. Local governments may use the findings to design more effective policies in areas like security and sanitation. Construction firms and investors can identify regions with higher growth and occupancy potential. The dataset includes demographic, economic, and environmental variables such as average number of rooms, building age, crime rate, pollution, distance to the city center, and residential taxes.

We will use **Python** and libraries like `pandas`, `numpy`, `scipy`, and `statsmodels` to perform hypothesis testing, regressions, and other statistical analyses. All work will be done in a Jupyter Notebook environment.Finally, key insights will be presented in an interactive **Power BI** dashboard, using **DAX** for creating analytical metrics—ensuring clear and actionable visualizations.

**Keywords**: Statistical Analysis, Business Analytics, Data Visualization, Python Language, Python Libraries, PowerBI, PowerQuery, DAX.

# ✅ PROCESS

We began the development with a detailed **Exploratory Data Analysis (EDA)** to understand the structure and distribution of the collected variables. In this phase, we used histograms and scatter plots to identify patterns and outliers. We observed that the dependent variable (**taxa_ocupacao**) had a slightly right-skewed distribution, indicating the possible presence of outliers. To reduce this distortion, we applied a logarithmic transformation, creating the variable **taxa_ocupacao_log**, which showed a distribution closer to normality, reducing skewness. Lastly, we also assessed the skewness of the other variables before proceeding with further analyses.

![Screenshot 2025-03-24 at 20 17 01](https://github.com/user-attachments/assets/cdcf10a1-ed05-4956-b912-0ea44857a74c)

In the next step, we performed a **Bivariate Analysis** to investigate the relationship between the dependent variable and each independent variable through a **correlation table**. We used the **Pearson correlation coefficient** to quantify the strength of linear relationships, identifying variables with greater predictive potential, such as the **average number of rooms per residence**, **crime rate**, and **distance to the city center**. Based on these results, we assessed the presence of **multicollinearity** among the independent variables using the **Variance Inflation Factor (VIF)**. This analysis allowed us to select only the most relevant and statistically reliable variables for the subsequent models.

![imagem1](https://github.com/user-attachments/assets/774015d8-21f0-48ad-92a1-15054f1f4ca6)

![imagem2](https://github.com/user-attachments/assets/29952055-944f-4c7d-826e-350faebc9b23)

Após identificar a necessidade de transformação dos dados, conduzimos também uma **remoção cuidadosa de outliers** através de análises gráficas e técnicas estatísticas, incluindo o teste de normalidade (**Shapiro-Wilk**) e avaliação da assimetria (**skewness**) das variáveis. Esta etapa garantiu que as análises subsequentes fossem realizadas sobre dados mais homogêneos e estatisticamente robustos. Com a base devidamente tratada, procedemos à construção dos **modelos de regressão linear múltipla**, sendo desenvolvidos cinco modelos distintos, cada um incorporando melhorias em relação ao anterior:

> **Modelo 1 (Dados Brutos)**: Serviu como modelo inicial para entender o comportamento geral dos dados sem ajustes adicionais.

> **Modelo 2 (Dados Padronizados)**: Incorporou técnicas de padronização dos dados para melhorar a interpretação e comparabilidade dos coeficientes.

> **Modelo 3 (Dados sem Multicolinearidade)**: Variáveis com alto VIF foram excluídas para mitigar os efeitos negativos da multicolinearidade.

> **Modelo 4 (Dados sem variáveis de baixa significância - primeira otimização)**: Variáveis com valores-p elevados (baixa significância estatística) foram excluídas.

> **Modelo 5 (Dados sem variáveis de baixa significância - otimização final)**: Uma otimização ainda mais rigorosa foi feita, reduzindo o modelo apenas às variáveis mais relevantes estatisticamente.

![212121](https://github.com/user-attachments/assets/c68c8608-b7df-48e8-a072-52990ae461cc)

Cada modelo foi cuidadosamente avaliado utilizando métricas importantes como o **valor-p**, essencial para determinar a significância das variáveis, e o **coeficiente R-Squared (R²)**, que indica o quanto cada modelo explica a variabilidade da taxa de ocupação dos imóveis. Durante toda a construção dos modelos, avaliamos rigorosamente as suposições fundamentais da regressão linear múltipla, que incluem: **Linearidade**, **Independência dos erros**, **Homocedasticidade**, **Normalidade dos erros** e **Ausência de multicolinearidade**.

![Screenshot 2025-03-24 at 20 48 18](https://github.com/user-attachments/assets/85b9e3c2-961d-4a44-91eb-7df31de13a2e)

Ao final, o quinto modelo, otimizado após todos esses ajustes, apresentou o melhor desempenho estatístico, permitindo identificar claramente os fatores que influenciam diretamente na taxa de ocupação dos imóveis.

# ✅ CONCLUSION

Neste projeto, constatamos que a multicolinearidade é um problema grave, pois pode comprometer significativamente a qualidade e confiabilidade dos modelos estatísticos, bem como tornar o modelo tendencioso. Para mitigar esse risco, utilizamos o **Fator de Inflação da Variância (VIF)**, identificando e removendo variáveis altamente correlacionadas entre si.

Após rigorosas análises estatísticas—como testes de Pearson, avaliação de valores-p e regressões lineares múltiplas—identificamos claramente os fatores mais relevantes para a taxa de ocupação dos imóveis: **número médio de quartos por residência**, **taxa de criminalidade**, **presença de rio no bairro**, **taxa de poluição**, **distância do centro da cidade**, **taxa de professores** e **taxa de desabrigados**.

Essas variáveis são determinantes para a ocupação imobiliária e podem ser utilizadas pela prefeitura na criação de políticas públicas de infraestrutura e segurança, bem como por investidores privados em decisões estratégicas de localização.

Por fim, com base nas variáveis mais relevantes identificadas, foi desenvolvido um dashboard interativo no Power BI, utilizando o PowerQuery para tratamento eficiente dos dados e a linguagem DAX para criação de métricas claras e objetivas, proporcionando ferramentas analíticas sólidas para tomada de decisões estratégicas.

**Dashboard**:


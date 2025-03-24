# ✅ PROJECT-06

Nesse projeto, realizaremos uma análise multivariada com o intuito de responder especificamente à pergunta: **"Quais fatores mais influenciam na taxa de ocupação de imóveis?"**. O projeto está sendo conduzido por uma empresa de tecnologia especializada em análise de dados e estatística, que está estudando detalhadamente diferentes bairros de uma determinada cidade. O objetivo é produzir análises completas que posteriormente possam ser comercializadas e aproveitadas por diferentes setores.

Responder a esta pergunta principal permitirá gerar insights valiosos que podem ser utilizados por diversas entidades. Por exemplo, a prefeitura poderá utilizar as informações obtidas para desenvolver políticas públicas mais eficientes relacionadas à segurança, distribuição de água e saneamento básico, impactando positivamente a qualidade de vida dos moradores. Da mesma forma, construtoras do setor privado poderão se beneficiar desses dados para decisões estratégicas de localização e investimento, identificando áreas com maior potencial de crescimento e ocupação. Além disso, investidores imobiliários poderão empregar essas análises para avaliar com maior precisão riscos e oportunidades antes de realizarem investimentos em regiões específicas.

Para alcançar esses objetivos, utilizaremos uma base de dados abrangente contendo variáveis demográficas, econômicas e ambientais, tais como número médio de quartos por residência, idade média das residências, taxa de criminalidade, proporção de empresas, presença de rios no bairro, taxas de poluição, distância do centro da cidade, acessibilidade, impostos residenciais, taxas de professores, consumo médio de energia e taxa de desabrigados.

Aplicaremos conceitos estatísticos rigorosos utilizando a linguagem **Python** e uma ampla gama de bibliotecas especializadas (como `pandas`, `numpy`, `scipy`, `statsmodels`, `matplotlib` e `seaborn`) para conduzir testes de hipótese, análises exploratórias profundas, regressões lineares, análise de variância (**ANOVA**) e demais análises necessárias para responder precisamente à pergunta central do projeto. Todo o código foi desenvolvido no Jupyter Notebook devido a quantidade considerável de análises, correções e otimizações feitas em várias etapas do processo de análise.

Por fim, utilizaremos o **Power BI** para criar um dashboard interativo, apresentando visualmente os principais indicadores e métricas obtidos durante a análise. Para garantir máxima eficiência e clareza nas visualizações, empregaremos também as linguagens **DAX** para criação de medidas analíticas precisas e **PowerQuery** para limpeza, transformação e otimização dos dados, garantindo relatórios assertivos e capazes de auxiliar diferentes setores na tomada de decisões estratégicas baseadas em dados.

**Keywords**: Statistical Analysis, Business Analytics, Data Visualization, Python Language, Python Libraries, PowerBI, PowerQuery, DAX.

# ✅ PROCESS

Iniciamos o desenvolvimento com uma **Análise Exploratória de Dados (EDA)** detalhada para compreender a estrutura e distribuição das variáveis coletadas. Nessa etapa, utilizamos histogramas e gráficos de dispersão para identificar padrões e outliers. Observamos que a variável dependente (**taxa_ocupacao**) apresentava uma distribuição levemente assimétrica à direita,  indicando possível presença de valores discrepantes (outliers). Para reduzir essa distorção, aplicamos uma transformação logarítmica, criando a variável **taxa_ocupacao_log**, que passou a apresentar uma distribuição mais próxima da normalidade, reduzindo a assimetria. Por fim, avaliamos também a assimetria das demais variáveis antes de avançar nas análises seguintes.

![Screenshot 2025-03-24 at 20 17 01](https://github.com/user-attachments/assets/cdcf10a1-ed05-4956-b912-0ea44857a74c)

Na sequência, realizamos uma **Análise Bivariada**, investigando a relação individual entre a variável dependente e cada uma das variáveis independentes através da criação de uma **tabela de correlação**. Foi aplicado o **coeficiente de Pearson** para quantificar o grau de correlação linear entre as variáveis, permitindo identificar rapidamente aquelas com maior potencial preditivo. Nesta etapa, destacaram-se variáveis como **número médio de quartos por residência**, **taxa de criminalidade**, e **distância do centro**, que apresentaram maior correlação com a taxa de ocupação.

![imagem1](https://github.com/user-attachments/assets/774015d8-21f0-48ad-92a1-15054f1f4ca6)

Diante dos resultados iniciais da correlação, avaliamos a presença de **multicolinearidade** entre as variáveis independentes, uma situação que pode comprometer a precisão e interpretação dos modelos estatísticos. Aplicamos rigorosamente o cálculo do **Fator de Inflação da Variância (VIF)** para identificar quais variáveis apresentavam alta correlação entre si. Isso nos permitiu fazer uma seleção criteriosa das variáveis mais apropriadas para inclusão nos modelos posteriores.

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


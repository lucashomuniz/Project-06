# ✅ PROJECT-06

Nesse projeto, realizaremos uma análise multivariada com o intuito de responder especificamente à pergunta: **"Quais fatores mais influenciam na taxa de ocupação de imóveis?"**. O projeto está sendo conduzido por uma empresa de tecnologia especializada em análise de dados e estatística, que está estudando detalhadamente diferentes bairros de uma determinada cidade. O objetivo é produzir análises completas que posteriormente possam ser comercializadas e aproveitadas por diferentes setores.

Responder a esta pergunta principal permitirá gerar insights valiosos que podem ser utilizados por diversas entidades. Por exemplo, a prefeitura poderá utilizar as informações obtidas para desenvolver políticas públicas mais eficientes relacionadas à segurança, distribuição de água e saneamento básico, impactando positivamente a qualidade de vida dos moradores. Da mesma forma, construtoras do setor privado poderão se beneficiar desses dados para decisões estratégicas de localização e investimento, identificando áreas com maior potencial de crescimento e ocupação. Além disso, investidores imobiliários poderão empregar essas análises para avaliar com maior precisão riscos e oportunidades antes de realizarem investimentos em regiões específicas.

Para alcançar esses objetivos, utilizaremos uma base de dados abrangente contendo variáveis demográficas, econômicas e ambientais, tais como número médio de quartos por residência, idade média das residências, taxa de criminalidade, proporção de empresas, presença de rios no bairro, taxas de poluição, distância do centro da cidade, acessibilidade, impostos residenciais, taxas de professores, consumo médio de energia e taxa de desabrigados.

Aplicaremos conceitos estatísticos rigorosos utilizando a linguagem **Python** e uma ampla gama de bibliotecas especializadas (como `pandas`, `numpy`, `scipy`, `statsmodels`, `matplotlib` e `seaborn`) para conduzir testes de hipótese, análises exploratórias profundas, regressões lineares, análise de variância (**ANOVA**) e demais análises necessárias para responder precisamente à pergunta central do projeto. Todo o código foi desenvolvido no Jupyter Notebook devido a quantidade considerável de análises, correções e otimizações feitas em várias etapas do processo de análise.

Por fim, utilizaremos o **Power BI** para criar um dashboard interativo, apresentando visualmente os principais indicadores e métricas obtidos durante a análise. Para garantir máxima eficiência e clareza nas visualizações, empregaremos também as linguagens **DAX** para criação de medidas analíticas precisas e **PowerQuery** para limpeza, transformação e otimização dos dados, garantindo relatórios assertivos e capazes de auxiliar diferentes setores na tomada de decisões estratégicas baseadas em dados.

**Keywords**: Statistical Analysis, Business Analytics, Data Visualization, Python Language, Python Libraries, PowerBI, PowerQuery, DAX.

# ✅ PROCESS

Criar imagens e explicar a análise de correlação de cada uma.
Método de Pearson é um teste estatístico paramétrico, para medir a correlação entre duas variáveis.

Perigo sobre Outliers, é necessário ser retirado. 
Criar texto/imagem sobre isso.

Modelo 1: Dados brutos
Modelo 2: Dados padronizados
Modelo 3: Dados sem multicolinearidade
Modelo 4: Sem variáveis de baixa significância
Modelo 5: 

Se o valor-p for maior que 0.05 é necessário deletar a variável, pois ela não é estatisticamente significativa para explicar a variável alvo.

# ✅ CONCLUSION

Multicolinearidade tem que ser revolvido. Multicolinearidade é um problema em regressão. Onde basicamente se está duplicando uma informação. Por exemplo, duas variáveis são altamente colineares, então basicamente aquela informação está duplicada/reforçada. Isso como consequência vai deixar o modelo tendêncioso.

**Dashboard**:


# ✅ PROJECT 11

Tem aumentado de forma contínua o número de pacientes com doença hepática devido ao consumo excessivo de álcool, inalação de gases nocivos, ingestão de alimentos contaminados e uso de drogas e anabolizantes. Neste Projeto objetivo é desenvolver um modelo de Machine Learning capaz de prever se um paciente vai ou não desenvolver uma doença hepática com base em diversas características do paciente. Esse modelo pode ajudar médicos, hospitais ou governos a planejar melhor o orçamento de gastos de saúde ou mesmo criar políticas de prevenção. O principal objetivo é prever uma classe (sim ou não), para isso usaremos aprendizado supervisionado de classificação, criando diferentes versões do modelo com diferentes algoritmos, passando por todo o processo de Machine Learning de ponta a ponta.

O objetivo é passar por todo o processo de construção, treinamento, avaliação e seleção de modelos para classificação. Para que possa compreender muito bem como funciona o processe, começando a partir de um problema de negócio, chegando até a entrega de um modelo treinado fazendo previsões. Respondendo perguntas como: Quais são as técnicas que devem ser empregada ao longo do processo?, Qual a ordem de aplicaçào dessas técncias?, Quais ferramentas você deve usar e quando? Se utilizar mais de um algoritmo como posso comparar as versões de cada um deles? 

Keywords: 

# ✅ PROCESS

Com base na definição do problema de negócio e olhando para o dataframe, é possível saber qual o algortimo ideal para desenvolver o mdoelo de machine learning? Na grande maioria das vezes a resposta é não. Com base nisso, o plano é começar com um processo de experimentação, na qual será testado alguns algoritmos com diferentes combinações de hiperparâmetros, criando diferentes versões dos modelos e depois comparar o que obteve a melhor performace. Antes de se começar o projeto, já se sabe quais são as técnicas ideias de pré-processamento? Na grande maioria das vezes a resposta é não. De forma semelhante, faremos o processo de experimentação. O trabalho do cientista de dados é com base no processo de experimentação escolher qual é o melhor algoritmo, a melhor técnica e a melhor estratégia. 

A Análise Exploratória é feita logo no início, após o carregamento dos dados. Nessa fase é feita toda o processo de limpeza (valores duplicados e valores ausentes), bem como possiveis transformações pontuais. O principal foco é realizar o entendimento do dataframe, com foco na visualização dos tipos das variáveis númerias e categóricas, bem como na visualização das suas distribuições e principalmente o tratamento de outliers a partir do boxplot, tabela de describe e contagem de frequência. Na Análise Exploratória não se pode ter linhas duplicadas nem colunas (variáveis) duplicadas, pelo fato de que caso isso ocorra teriamos uma dupicidade, o que teoricamente iria fazer com que o modelo desenvolvido fosse tendecioso, pois estariamos reforçando uma informação. O objetivo é ter um modelo generalizável.

A etapa seguinte é o processo de Engenharia de Atributos, na qual é desenvolvido um tipo de transformação mais profunda (caso necessário) bem como uma possível criação e alteração das variáveis. Uma opção dentre dess fase é fazer o Feature Selection, com o intuito de obter as melhores variáveis para seguir com o processo de Machine Learning. Por fim, uma das técnicas mais importantes nessa fase é a criacão da Tabela de Correlação, na qual vai ser possível identificar possíveis níveis (positivo ou negativo) de relacionamento entre as variáveis, pricipalmente analisar possíveis indícios de multicolinearidade entre variáveis.

Sequencialmente, a etapa de Análise Estatística é baseada no teorema do limite central, desenvolvendo teste de hipóteses entre variáveis, teste de shapiro-wilker, teste-t, teste-f, teste anova e regressão linear.

A proxima etapa é o pré-processamento, onde é feito as alterações de variáveis que tenham ainda texto para número, bem como é feito a organização de todo o modelo de machine learning, escolha do algoritmo principal, label enconding, normalização, padronizaçào e scaling. Uma outra técnica bastante utilizada durante essa etapa é de dividr os dados do dataframe em dados de treino e dados de teste. Isso é importante pelo fato de que o modelo de machine learning é treinado (criado) com os dados de treino e em seguida é testadado (avaliado) com os dados de teste. Uma vez que o modelo esteja treinado, eu não posso apresentar a ele os mesmos dados utilizados em treinamento, porque ele já conhece esses dados. Para avaliar a performace do modelo, eu tenho que utilizar novos dados que eu obviamente já conheco o resultado

# ✅ CONCLUSION

O primeiro modelo a ser criado é o modelo base, normalmente é escolhido um algoritmo que seja simples e fácil de interpretar. A Regressão Logística (Benchmark) é  uma ótima opção quando trabalhamos com regressão. O Bechmark é muito útil pelo fato de além de entregar a classe do modelo de classificação, ainda calcula a probabilidade.

<img width="613" alt="image" src="https://github.com/lucashomuniz/Project-11/assets/123151332/d30b0939-b1a8-460f-8d8a-abe09277e610">


Random Forest

KNN

Decision Tree

SVM


















# ✅ DATA SOURCES

Usaremos como fonte de dados o dataset disponível no link: https://archive.ics.uci.edu/dataset/225/ilpd+indian+liver+patient+dataset

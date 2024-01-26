# DAA-Dados e Aprendizagem Automática
Este repositório contém conteúdo relativo à Unidade Curricular de Dados e Aprendizagem Automática, inserido no 1º Ano e 1º Semestre do Mestrado em Engenharia Informática.
Este Trabalho por Realizado por : 

#### Afonso Bessa -pg53597
#### Hugo Martins - a95125
#### Ivo Ribeiro -pg53886
#### João Escudeiro-a96075

O trabalho consistia na aplicação de algoritmos de machine learning a dois conjuntos de  dados provenientes do mundo real.
Foi seguida uma metodologia semelhante à que está representada na figura abaixo.
![Metodologia](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/raw/main/Photos/Metodologia.png)


## Dataset Smoking and Drinking
Este Dataset era relativo a um ano na Coreia do Sul e continha informações de saúde relativas a um milhao de pessoas.
O maior objetivo seria prever se um paciente fuma ou bebe , baseado em dados de saúde como pressão arterial, nivel de visao, peso.altura,diabetes,colesterol.
Inicialmente realizamos uma análise de dados para verificar como estavam distribuídos os mesmos, bem como qual era a correlação das features com o nosso target.
Podemos observar a distribuição de features como a idade, a altura e o peso nas figuras abaixo.

![Boxplot](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/raw/main/Photos/boxplot.png)

![Countplot](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/countplot.png)

### Análise de correlação
![Correlation Matrix](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/C_Smoking.png)

Após realizar esta análise removemos alguns outliers, bem como incluímos novas features para passar para a fase de modelação.
Na fase de modelação os melhores resultados , bem como hiperparâmetros utilizados estao descritos na tabela abaixo.

![Drinking](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/Modelacao_Drinking.png) | ![Smoking](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/mODELACAO_SMOKING.png)


## Dataset Energy and weather
Foram nos fornecidos vários datasets, cujo conteúdo assentava na produção energética e o objetivo seria prever, através de dados meteorológivos e energéticos que nos foram fornecidos qual seria a quantidade de energia que poderia ser injetada na rede proveniente de uma habitação.
Assim foi necessário realizar vários passos como análise de dados, análise de correlação, criação de novas features.

Inicialmente optamos por juntar todos os dados em dois datframes, um que continha os dados de energia e meteorologia de teste e o outro continha os dados para treino.

Após isto Analisamos a qualidade dos dados para verificar se existia ou não Missing Values ou Duplicated Rows.
Removemos colunas com muitos missing values e analisamos a correlação com a target "Injection".
 ![Correlation Matrix](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/comp_corr_antes%20pp.png)

Realizaram-se alguns graficos para analisar a dispersão dos dados.

![Grafico123](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/grafico123.png)

![Barcharts](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/barcharts.png)

![Big Graph](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/big%20graph_comp.png)


O passo seguinte foi remover as colunas com baixa correlação, bem como incluir novas features que permitissem obter mais informação sobre o problema em questão.
Após realizar diversas procuras, decidimos incluir algumas colunas como períodos de férias, estações do ano, períodos de sol, tentativas de previsão da injeção.
Assim conseguimos adicionar informação muito importante para a previsão da injeção.
Os resultados obtidos na modelação foram:

![Accuracy Kaggle](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/Accuracy%20Kaggle.png)

![Accuracy Comparison](https://github.com/jbtescudeiro16/Dados-e-Aprendizagem-Automatica/blob/main/Photos/Accuracy_Comp.png)


## Conclusão

Este trabalho foi bastante útil para ficarmos familisarizados com técnicas de Machine Learning, bem como bibliotecas como pandas,seaborn , entre outras.
Para executar o trabalho basta baixar os notebooks e os datasets e executá-los de forma sequencial seguindo a ordem incluida nos Ficheiros.



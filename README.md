# Notebook de Análise e Modelagem de Churn

Este notebook contém os desafios propostos para a análise exploratória, pré-processamento e modelagem de um conjunto de dados de churn de clientes.

## Conteúdo

- **Aula 1: Obtenção e Limpeza de Dados**
  - Leitura da base de dados `churn.csv`.
  - Verificação da presença de dados nulos.
  - Análise exploratória inicial com `dados.info()` e visualização das primeiras linhas.

- **Aula 2: Pré-processamento de Dados**
  - Separação das variáveis explicativas (`x`) e variável alvo (`y`).
  - Transformação de variáveis categóricas para numéricas utilizando `OneHotEncoder` com `drop='if_binary'`.
  - Transformação da variável alvo `churn` utilizando `LabelEncoder`.

- **Aula 3: Modelagem e Avaliação (Modelos de Base e Árvore de Decisão)**
  - Divisão dos dados em conjuntos de treinamento e teste de forma estratificada.
  - Criação e avaliação de um modelo de base (`DummyClassifier`).
  - Criação e avaliação de um modelo de Árvore de Decisão (`DecisionTreeClassifier`) com `max_depth=4`.
  - Visualização da árvore de decisão.

- **Aula 4: Modelagem e Avaliação (KNN) e Salvamento de Modelos**
  - Normalização dos dados utilizando `MinMaxScaler`.
  - Criação e avaliação de um modelo KNN (`KNeighborsClassifier`) com dados normalizados.
  - Comparação das acurácias dos modelos `DummyClassifier`, `DecisionTreeClassifier` e `KNeighborsClassifier`.
  - Salvamento do melhor modelo (`DecisionTreeClassifier`) e do transformador (`OneHotEncoder`) utilizando `pickle`.
  - Carregamento dos modelos salvos e realização de uma previsão com um novo registro de dados.

## Como usar

1.  Execute as células do notebook sequencialmente para seguir o fluxo de análise e modelagem.
2.  Adapte o código conforme necessário para seus próprios conjuntos de dados ou experimentos.

# BaseDeHits

## Descrição do Projeto
Este projeto é uma análise preditiva e de segmentação de dados musicais, utilizando **modelos supervisionados e não supervisionados**. O foco é aplicar diferentes técnicas de **machine learning** para prever e agrupar músicas com base em suas características sonoras, identificando músicas com maior probabilidade de se tornarem hits.

## Modelos Utilizados
Neste projeto, foram implementados dois tipos de modelos:

### Modelos Supervisionados:
1. **KNN (K-Nearest Neighbors)**: Algoritmo de classificação baseado na proximidade entre os dados.
2. **SVC (Support Vector Classifier)**: Classificador que separa os dados utilizando hiperplanos com maior margem.
3. **Decision Tree**: Estrutura hierárquica de decisões que divide os dados em diferentes classes.
4. **Random Forest**: Modelo de conjunto que utiliza várias árvores de decisão para melhorar a performance do modelo.
5. **Logistic Regression**: Modelo que prevê a probabilidade de um determinado evento, usado aqui para classificação binária de hits.

### Modelos Não Supervisionados:
1. **K-Means**: Algoritmo de clustering que agrupa os dados com base na proximidade de características, formando clusters.
2. **GMM (Gaussian Mixture Model)**: Modelo que assume que os dados foram gerados a partir de uma combinação de várias distribuições normais, formando clusters de forma probabilística.

## Dataset
O DataFrame utilizado neste projeto contém informações detalhadas sobre músicas e suas características sonoras. Algumas das variáveis usadas para a análise incluem:

- **Danceability** (Dançabilidade)
- **Energy** (Energia)
- **Key** (Tom)
- **Loudness** (Volume)
- **Speechiness** (Presença de fala)
- **Acousticness** (Acústica)
- **Instrumentalness** (Instrumentalidade)
- **Liveness** (Vivacidade)
- **Valence** (Positividade emocional)
- **Tempo** (BPM)
- **Popularity** (Popularidade da música)

O DataFrame pode ser acessado diretamente [aqui](https://www.kaggle.com/datasets/thebumpkin/10400-classic-hits-10-genres-1923-to-2023).

## Análises Preditivas
### Predição de Hits
Foram aplicados os **5 modelos supervisionados** mencionados para a predição de hits musicais, com base na variável de **popularidade**. Os modelos foram ajustados e avaliados usando métricas de performance como **Acurácia**, **R²**, **Mean Squared Error (MSE)**, **Mean Absolute Error (MAE)** e **AUC-ROC**.

### Segmentação de Músicas
Os **modelos não supervisionados (K-Means e GMM)** foram aplicados para realizar a **segmentação de músicas** com base nas características acústicas e de popularidade, criando agrupamentos (clusters) que permitem uma análise mais detalhada sobre padrões musicais.

## Métricas Avaliativas
Para os modelos **supervisionados**, foram utilizadas as seguintes métricas:

- **Acurácia**: Mede a proporção de previsões corretas.
- **R²**: Indica a qualidade da previsão em relação à média dos dados.
- **Mean Squared Error (MSE)**: Avalia a média dos erros ao quadrado.
- **Mean Absolute Error (MAE)**: Mede a média dos erros absolutos.
- **AUC-ROC**: Avalia a capacidade do modelo em distinguir entre classes.

Para os modelos **não supervisionados**, foram utilizadas as seguintes métricas:

- **Silhouette Score**: Avalia a separação entre os clusters (quanto maior, melhor).
- **Davies-Bouldin Index**: Mede a separação dos clusters (quanto menor, melhor).
- **Calinski-Harabasz Index**: Avalia a dispersão dentro dos clusters (quanto maior, melhor).

Essas métricas ajudam a determinar a qualidade dos agrupamentos gerados pelos modelos **K-Means** e **GMM**.

## Referências
Para a criação deste projeto, utilizei como referência o notebook **Medical Insurance Price Prediction** e o meu próprio notebook **BaseDeHits**, que pode ser acessado [aqui](https://www.kaggle.com/code/kevinsouza284/basedehits).

## Conclusão
Este projeto foi um grande passo no desenvolvimento das minhas habilidades em **ciência de dados** e **machine learning**, tanto em **aprendizado supervisionado** quanto **não supervisionado**. Ao longo do projeto, foi possível experimentar diferentes abordagens e avaliar a performance de cada uma delas. Planejo continuar refinando este projeto, trazendo novos modelos e realizando mais análises preditivas e de clustering no futuro.

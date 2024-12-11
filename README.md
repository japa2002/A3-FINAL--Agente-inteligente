# A3-FINAL--Agente-inteligente

## Visão Geral
Este projeto implementa diversos algoritmos de classificação para analisar um dataset de dados médicos, utilizando técnicas de ensemble e modelos baseados em gradiente. Ele avalia o desempenho de cada modelo com base em métricas como acurácia, precisão, recall e F1-Score, além de gerar matrizes de confusão e visualizações comparativas.

## Requisitos do Sistema
- Python 3.7 ou superior
- Bibliotecas Python:
  - pandas
  - numpy
  - scikit-learn
  - seaborn
  - matplotlib
  - xgboost
  - lightgbm
  - catboost

Para instalar as dependências, use o seguinte comando:
```bash
pip install pandas numpy scikit-learn seaborn matplotlib xgboost lightgbm catboost
```

## Estrutura do Projeto
- **Dataset**: O arquivo CSV `diabetic_data.csv` deve estar localizado no caminho especificado no código. Ele contém dados médicos sobre pacientes diabéticos, incluindo informações demográficas, histórico de hospitalizações e resultados clínicos.
- **Código Python**: O script realiza:
  1. Carregamento e processamento do dataset.
  2. Codificação one-hot para variáveis categóricas.
  3. Normalização das variáveis independentes.
  4. Divisão dos dados em treino e teste.
  5. Treinamento e avaliação de vários modelos de classificação.

## Modelos Avaliados
1. Random Forest
2. Gradient Boosting
3. LightGBM
4. XGBoost
5. CatBoost
6. Extra Trees
7. Bagging
8. AdaBoost
9. Decision Tree
10. Voting Classifier (combinação de modelos principais com votação soft)

## Etapas Principais
1. **Carregamento e Validação do Dataset**:
   - Garante que todas as colunas necessárias estejam presentes.
   - Remove valores ausentes e codifica variáveis categóricas.
2. **Treinamento de Modelos**:
   - Cada modelo é treinado e testado separadamente.
3. **Avaliação de Desempenho**:
   - As métricas incluem:
     - Acurácia
     - Precisão
     - Recall
     - F1-Score
   - Relatórios de classificação e matrizes de confusão são gerados.
4. **Comparativo de Modelos**:
   - Resultados das métricas são exibidos em um gráfico para análise visual.

## Uso
1. Atualize o caminho do arquivo `diabetic_data.csv` no código:
   ```python
   file_path = "seu/caminho/para/diabetic_data.csv"
   ```
2. Execute o script em um ambiente Python ou Google Colab.
3. Observe os resultados no terminal e nas visualizações geradas.

## Resultados
- O script compara o desempenho de todos os modelos de classificação.
- Gera visualizações claras para identificar o melhor modelo com base nas métricas escolhidas.

## Observações
- O dataset precisa conter informações sobre hospitalizações e diagnósticos para um funcionamento adequado.
- Os parâmetros dos modelos podem ser ajustados para melhor desempenho em diferentes cenários.

## Contribuições
Contribuições para melhorias no código são bem-vindas! Sinta-se à vontade para abrir um *pull request* ou relatar problemas.

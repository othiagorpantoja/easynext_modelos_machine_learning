# Ajuste de Hiperparâmetros e Seleção de Features

Este projeto demonstra técnicas avançadas de otimização de modelos de machine learning, incluindo **Grid Search** para ajuste de hiperparâmetros e **Seleção de Features** para identificar as características mais relevantes.

## 📋 Conteúdo

### 1. Grid Search para Classificação
- **Dataset**: California Housing (transformado em problema de classificação)
- **Modelo**: Árvore de Decisão
- **Técnica**: Grid Search com validação cruzada
- **Objetivo**: Encontrar os melhores hiperparâmetros para maximizar a acurácia

### 2. Seleção de Features para Regressão
- **Dataset**: Pima Indians Diabetes (transformado em problema de regressão)
- **Modelo**: Random Forest
- **Técnicas**: F-Score, Mutual Information, Feature Importance
- **Objetivo**: Identificar as features mais importantes para previsão

## 🚀 Como Usar

### Pré-requisitos
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Executando o Notebook
1. Abra o arquivo `ajuste_hiperparametros_e_selecao_features.ipynb` no Google Colab
2. Execute todas as células sequencialmente
3. Observe os resultados e visualizações

## 📊 Técnicas Implementadas

### Grid Search
- **Hiperparâmetros testados**:
  - `max_depth`: [3, 5, 7, 10, None]
  - `min_samples_split`: [2, 5, 10, 20]
  - `min_samples_leaf`: [1, 2, 4, 8]
  - `criterion`: ['gini', 'entropy']
  - `max_features`: ['sqrt', 'log2', None]

### Seleção de Features
1. **F-Score**: Mede relação linear entre features e variável alvo
2. **Mutual Information**: Captura dependências não-lineares
3. **Feature Importance**: Baseado na redução de impureza (Random Forest)

## 📈 Resultados Esperados

### Classificação (California Housing)
- Comparação entre modelo base e otimizado
- Matriz de confusão
- Importância das features
- Melhoria na acurácia

### Regressão (Pima Indians Diabetes)
- Comparação de diferentes métodos de seleção
- Análise de correlação entre features
- Performance com diferentes números de features
- Visualizações comparativas

## 🔍 Insights Principais

1. **Grid Search** pode melhorar significativamente o desempenho do modelo
2. **Diferentes métodos** de seleção de features podem identificar características distintas
3. **Seleção de features** pode manter ou melhorar a performance com menos variáveis
4. **Validação cruzada** é essencial para uma avaliação robusta

## 📁 Estrutura do Projeto

```
easynext_modelos_machine_learning/
├── README.md
└── ajuste_hiperparametros_e_selecao_features.ipynb
```

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- **Pandas**: Manipulação de dados
- **NumPy**: Computação numérica
- **Matplotlib/Seaborn**: Visualizações
- **Scikit-learn**: Machine learning
- **Google Colab**: Ambiente de execução

## 📚 Conceitos Aprendidos

### Ajuste de Hiperparâmetros
- Como usar Grid Search
- Validação cruzada
- Comparação de modelos
- Interpretação de resultados

### Seleção de Features
- Métodos estatísticos (F-Score)
- Métodos baseados em informação (Mutual Information)
- Métodos baseados em árvores (Feature Importance)
- Análise de correlação

## 🎯 Próximos Passos

Para continuar explorando:
1. Testar outros algoritmos de seleção de features
2. Aplicar técnicas de redução de dimensionalidade (PCA, LDA)
3. Experimentar com diferentes números de features selecionadas
4. Usar validação cruzada para uma avaliação mais robusta
5. Implementar Random Search como alternativa ao Grid Search

## 📖 Referências

- [Scikit-learn Grid Search](https://scikit-learn.org/stable/modules/grid_search.html)
- [Feature Selection in Scikit-learn](https://scikit-learn.org/stable/modules/feature_selection.html)
- [California Housing Dataset](https://scikit-learn.org/stable/datasets/real_world.html#california-housing-dataset)
- [Pima Indians Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

## 👥 Contribuições

Este projeto foi desenvolvido como parte do curso de Machine Learning da EasyNext. Sinta-se à vontade para sugerir melhorias ou adicionar novas funcionalidades!

---

**Desenvolvido com ❤️ para o aprendizado de Machine Learning**

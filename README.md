# Projeto de Inteligência Artificial — Classificação e Agrupamento de Dados

Este repositório contém um trabalho desenvolvido para a disciplina de Inteligência Artificial, com foco em técnicas de aprendizado supervisionado e não supervisionado utilizando a biblioteca scikit-learn.

## Objetivo

Aplicar e comparar algoritmos de:

- **Classificação** (aprendizado supervisionado)
- **Agrupamento** (aprendizado não supervisionado)

utilizando o dataset Zoo da UCI Machine Learning Repository.

## Dataset

O conjunto de dados utilizado possui:

- 101 animais
- 16 atributos
- 7 classes diferentes de animais

Foi criada uma versão modificada do dataset removendo os atributos:

- `hair`
- `feathers`

O objetivo foi analisar o impacto dessa modificação nos modelos de aprendizado de máquina.

## Técnicas Utilizadas

### Classificação
- Algoritmo: Random Forest
- Métricas utilizadas:
  - Classification Report
  - Matriz de Confusão

### Agrupamento
- Algoritmo: K-Means
- Métrica utilizada:
  - Silhouette Score

## Bibliotecas Utilizadas : 

pandas, numpy, matplotlib, seaborn, scikit-learn, ucimlrepo

## Resultados

### Random Forest
Os resultados de classificação permaneceram praticamente idênticos entre o dataset original e o modificado, indicando forte correlação entre os atributos removidos e os atributos restantes.

### K-Means
O dataset modificado apresentou uma pequena redução no Silhouette Score, mostrando que a remoção dos atributos prejudicou a separação natural dos grupos.

## Estrutura do Projeto

- `atividade_ia.ipynb` → Notebook principal contendo todo o desenvolvimento do trabalho
- `README.md` → Descrição do projeto

## Conclusão

O trabalho demonstrou como alterações nos atributos de um dataset podem impactar diferentes tipos de modelos de aprendizado de máquina. Enquanto o Random Forest conseguiu manter o desempenho devido à redundância das informações, o K-Means apresentou perda na qualidade dos agrupamentos após a remoção dos atributos.

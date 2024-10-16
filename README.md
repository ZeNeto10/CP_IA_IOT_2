# Projeto de Detecção de Diabetes e Classificação

## Descrição do Projeto

Este projeto é focado na detecção de diabetes através de dois modelos de aprendizado de máquina: uma rede neural artificial e um classificador K-Nearest Neighbors (KNN). O objetivo é prever a presença de diabetes em pacientes com base em várias características médicas, utilizando dados de um conjunto de dados conhecido.

## Objetivos

- **Detecção de Diabetes:** Criar modelos que possam prever se um paciente tem diabetes, fornecendo uma ferramenta útil para profissionais de saúde.
- **Comparação de Modelos:** Avaliar o desempenho de uma rede neural em comparação com um modelo KNN, ambos aplicados ao mesmo conjunto de dados.

## Detalhes dos Modelos

### 1. Rede Neural Artificial

A rede neural foi implementada utilizando a biblioteca PyTorch. O modelo é composto por:

- **Camadas:** Três camadas totalmente conectadas (fully connected) com funções de ativação ReLU nas camadas ocultas e uma função de ativação sigmoide na camada de saída para produzir uma probabilidade entre 0 e 1.
- **Função de Perda:** Utiliza a função de perda binária (BCELoss), que é adequada para tarefas de classificação binária.
- **Otimização:** O otimizador Adam é utilizado para atualizar os pesos da rede durante o treinamento.

**Arquitetura da Rede Neural:**
- **Camada de Entrada:** 8 neurônios (correspondendo ao número de características de entrada).
- **Camada Oculta:** 16 neurônios.
- **Camada de Saída:** 1 neurônio (resultado da predição).

### 2. Classificador K-Nearest Neighbors (KNN)

O classificador KNN foi implementado usando a biblioteca scikit-learn. O modelo KNN é um algoritmo simples e eficaz que classifica um ponto de dados com base na maioria dos rótulos dos seus K vizinhos mais próximos.

- **Parâmetro K:** O número de vizinhos a serem considerados é definido como 5. Este parâmetro pode ser ajustado para otimizar o desempenho do modelo.
- **Normalização:** Os dados são normalizados antes do treinamento para garantir que todas as características tenham o mesmo peso durante o cálculo das distâncias.

## Conjunto de Dados

O conjunto de dados utilizado para o treinamento e teste dos modelos é o "diabetes.csv", que contém informações sobre pacientes, incluindo características como:

- Idade
- Índice de Massa Corporal (IMC)
- Nível de glicose
- Pressão arterial
- Nível de insulina
- e outras variáveis relevantes.

O objetivo é prever a coluna "Outcome", que indica a presença (1) ou ausência (0) de diabetes.

## Resultados

Após a execução dos modelos, são exibidas as métricas de desempenho, incluindo a acurácia dos modelos. A comparação entre os dois métodos permite identificar qual deles oferece melhores resultados para a detecção de diabetes.

## Conclusão

Este projeto demonstra a aplicação de técnicas de aprendizado de máquina na área da saúde, com foco na detecção precoce de diabetes. A implementação de diferentes modelos permite não apenas a previsão de resultados, mas também uma compreensão mais profunda sobre o desempenho de algoritmos de aprendizado de máquina em um contexto real.




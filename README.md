# 🧠 Otimização de Hiperparâmetros com Algoritmos Evolutivos em MLPClassifier

Este projeto faz parte da disciplina de **Inteligência Artificial** e tem como objetivo aplicar **algoritmos evolutivos**, mais especificamente **algoritmos genéticos**, para otimizar os hiperparâmetros de um classificador MLP (Multi-Layer Perceptron) utilizando a biblioteca `scikit-learn`.

---

## 📂 Estrutura do Projeto

- `Algoritmos_Evolutivos_Rafael.ipynb`: Notebook principal contendo toda a implementação, análise e visualização.
- `Figure_2.1.png`: Gráfico das curvas de loss (Treinamento vs Validação) do modelo final.

---

## 🧬 Técnicas Utilizadas

- **Algoritmos Genéticos (DEAP)**: Utilizados para busca dos melhores hiperparâmetros do modelo.
- **MLPClassifier (Scikit-learn)**: Rede neural feedforward para classificação supervisionada.
- **Validação Cruzada e Early Stopping**: Para garantir melhor generalização e prevenir overfitting.
- **Visualização das Curvas de Loss**: Para avaliação do comportamento do modelo durante o treinamento.

---

## ⚙️ Hiperparâmetros Otimizados

Durante o processo evolutivo, os seguintes hiperparâmetros foram ajustados:

- `learning_rate_init`
- `hidden_layer_sizes`
- `activation`
- `solver`
- `max_iter`

O algoritmo buscou a melhor combinação com base no **F1-score** da validação.

---

## 📈 Avaliação de Desempenho

O modelo final foi avaliado utilizando:

- **F1-Score**
- **Precisão**
- **Recall**

Essas métricas foram calculadas sobre o **conjunto de teste**, contendo dados não vistos durante o treinamento/validação.

---

## 📊 Análise das Curvas de Loss

O notebook inclui a visualização da **loss de treinamento** (via `loss_curve_`) e uma **loss de validação aproximada**, estimada com base na acurácia (usando `1 - acurácia`). Essa análise permite:

- Detectar overfitting;
- Avaliar a estabilidade do treinamento;
- Observar a convergência do modelo ao longo das épocas.

---

## 📝 Conclusão

O uso de algoritmos genéticos se mostrou eficaz para a otimização dos hiperparâmetros do MLPClassifier, resultando em um modelo com bom desempenho e capacidade de generalização. Apesar do maior custo computacional, a abordagem oferece uma alternativa poderosa à busca manual ou exaustiva.

---

## 📚 Tecnologias e Bibliotecas

- Python 3.x
- Scikit-learn
- DEAP
- NumPy
- Matplotlib

---

## 👨‍💻 Autor

Rafael Diniz  
Disciplina: INTELIGÊNCIA ARTIFICIAL 
Professor(a): THALES LEVI AZEVEDO VALENTE 
Instituição: Universidade Federal do Maranhão 











# test_ICMC
Aplicação de dois modelos de classificação dos dados com o uso do dataset iris

Acerca do dataset

O conjunto de dados Iris é um dos mais populares e amplamente utilizados em aprendizado de máquina e estatística, especialmente para resolver problemas de classificação. Ele foi compilado por Ronald A. Fisher em 1936 e reúne informações sobre três espécies de flores do gênero Iris:

    Iris setosa
    Iris versicolor
    Iris virginica

Este dataset possui 150 amostras, distribuídas de forma igual entre as três espécies de flores (50 amostras para cada espécie). Cada amostra contém 4 características numéricas, medidas em centímetros, que descrevem aspectos morfológicos das flores. Essas características são:

    SepalLengthCm: Comprimento da sépala
    SepalWidthCm: Largura da sépala
    PetalLengthCm: Comprimento da pétala
    PetalWidthCm: Largura da pétala

Além das características acima, o conjunto de dados inclui a coluna Species, que representa o rótulo de classificação, indicando a espécie correspondente a cada flor.

Modelos utilizados

1. SVM (Support Vector Machine)
O SVM é um algoritmo de aprendizado supervisionado que busca encontrar o hiperplano ideal que separa as classes em um espaço de características.
É particularmente útil para problemas de classificação e funciona bem em casos onde as classes não são linearmente separáveis.

2. Regressão Logistica
Apesar do nome, Logistic Regression não é um algoritmo de regressão, mas sim de classificação.
Ele é usado para prever a probabilidade de uma amostra pertencer a uma classe específica (por exemplo, "sim" ou "não").

Em nosso teste 
Resultados por Modelo:
SVM (Support Vector Machine):

Acurácia: 97%
O modelo classificou corretamente 97% das amostras no conjunto de teste.
Desempenho por classe:
        Iris-setosa: Precision, Recall e F1-score de 1.00 significam que a classe foi identificada perfeitamente.
        Iris-versicolor: Recall de 0.89 indica que 11% das amostras dessa classe foram classificadas incorretamente.
        Iris-virginica: Recall de 1.00 e Precision de 0.92 mostram que todas as amostras dessa classe foram identificadas, mas houve algumas confusões com outras classes.

Regressão Logística:

Acurácia: 100%
O modelo conseguiu classificar corretamente todas as amostras no conjunto de teste.
Desempenho por classe:
        Todas as métricas (Precision, Recall e F1-score) têm valor de 1.00 para cada classe, indicando que o modelo não cometeu erros.

Resumo:

O modelo de Regressão Logística teve um desempenho perfeito no conjunto de teste.
O modelo SVM teve um desempenho levemente inferior, com acurácia de 97%. A principal limitação foi no recall da classe Iris-versicolor.

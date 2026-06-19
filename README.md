# KNN

Um dos algoritmos mais intuitivos de ML: para classificar um ponto novo, o modelo simplesmente olha para os K vizinhos mais próximos no espaço de features e vota na classe mais comum entre eles. Sem treino explícito, tudo acontece na hora da predição.

Exercício focado em entender como a escolha do K e a métrica de distância afetam o resultado.

# No notebook


Exploração e normalização dos dados (etapa crítica pro KNN, que é sensível à escala)
Treinamento com KNeighborsClassifier do scikit-learn
Busca pelo K ideal testando diferentes valores e plotando a curva de acurácia
Avaliação com métricas de classificação e visualização da fronteira de decisão

KNN não aprende nada durante o "treino", ele só memoriza os dados. O custo real vem na predição, quando precisa calcular a distância do ponto novo para todos os pontos do dataset. Por isso normalizar as features antes é essencial: se uma variável tem escala muito maior que as outras, ela domina o cálculo de distância e distorce o resultado.

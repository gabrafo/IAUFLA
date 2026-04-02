# Projeto 1 IA - KNN

## Contexto do projeto

Este relatório descreve a solução desenvolvida para o Projeto 1 da disciplina de Inteligência Artificial da UFLA, com foco no algoritmo K-Nearest Neighbors (KNN). A proposta foi implementar o método de classificação de forma manual e, em paralelo, comparar o comportamento dessa implementação com a versão disponibilizada pela biblioteca scikit-learn, observando desempenho, qualidade das predições e aspectos de eficiência.

## Objetivo da solução

A solução foi estruturada para demonstrar, de forma clara, como o KNN funciona na prática e como as escolhas de projeto afetam os resultados. O trabalho buscou validar os resultados da implementação própria por meio de uma referência consolidada, além de discutir variações de parâmetro, especialmente diferentes valores de k, e os efeitos dessas escolhas sobre a classificação.

## Metodologia adotada

A base de dados utilizada foi dividida em conjuntos de treino e teste, preservando um fluxo de avaliação padronizado. Na implementação manual, a classificação de cada amostra foi feita a partir do cálculo de distância euclidiana para os elementos do conjunto de treino, seguido da escolha dos vizinhos mais próximos e votação majoritária da classe prevista. Na implementação com scikit-learn, foi utilizado o `KNeighborsClassifier`, mantendo os mesmos conjuntos para que a comparação fosse justa.

Foram avaliados os valores de k iguais a 1, 3, 5 e 7. Para cada configuração, foram construídas matrizes de confusão e calculadas métricas de acurácia e revocação, permitindo uma leitura consistente da qualidade do classificador.

## Implementação e comparação

A implementação manual cumpriu o papel de explicitar os fundamentos do algoritmo, especialmente as etapas de cálculo de distância e decisão por votação. Já a implementação com scikit-learn ofereceu uma interface mais direta, com menor complexidade de código e maior robustez para experimentação.

A comparação entre as duas abordagens mostrou que os resultados tendem a ser próximos quando os mesmos dados e parâmetros são utilizados, mas a versão da biblioteca se destaca em manutenção, legibilidade e disponibilidade de recursos adicionais para escalabilidade.

## Otimizações analisadas

Também foi considerada a discussão sobre estratégias de busca de vizinhos presentes no scikit-learn, como `brute`, `kd_tree`, `ball_tree` e `auto`. O trabalho destaca que, em conjuntos pequenos e de baixa dimensionalidade, as diferenças de tempo de execução costumam ser discretas. Em cenários maiores, no entanto, estruturas de árvore podem reduzir custo de busca, dependendo da distribuição dos dados e da dimensionalidade do problema.

## Resultados observados

Os testes com diferentes valores de k permitiram verificar o comportamento esperado do algoritmo: valores muito baixos podem aumentar sensibilidade a ruído, enquanto valores mais altos tendem a suavizar a fronteira de decisão. As métricas calculadas e os gráficos gerados reforçaram essa leitura e serviram como base para a conclusão do projeto.

## Conclusão

A solução desenvolvida atendeu ao objetivo de estudar o KNN de forma conceitual e aplicada. A implementação manual foi importante para consolidar entendimento técnico, e a comparação com scikit-learn trouxe uma visão prática sobre produtividade e confiabilidade em contexto real de desenvolvimento. O projeto também permitiu discutir critérios de escolha de parâmetros e alternativas de otimização, conectando teoria e prática de forma coerente.

## Integrantes

- Gabriel Fagundes M. Sousa
- Hugo Dias Pontello

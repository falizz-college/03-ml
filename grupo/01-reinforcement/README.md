# Otimização do Algoritmo Random Forest

Este projeto apresenta um estudo sobre a aplicação e otimização do algoritmo **Random Forest**, utilizando um dataset de classificação de vinhos para avaliar o impacto de diferentes técnicas de ajuste de hiperparâmetros no desempenho do modelo.

## Visão Geral
O projeto foi desenvolvido como parte da disciplina de Engenharia de Software no **IDP** (Instituto Brasileiro de Ensino, Desenvolvimento e Pesquisa). O objetivo central foi investigar se métodos de busca de hiperparâmetros poderiam elevar a acurácia inicial de um modelo já estável.

## Metodologia

### Algoritmo Utilizado
O Random Forest foi selecionado por sua robustez e eficácia em reduzir o *overfitting* através da combinação de múltiplas árvores de decisão.

### Técnicas de Otimização
Foram aplicados três métodos distintos para explorar as melhores combinações de hiperparâmetros:
* **Randomized Search**
* **Bayesian Search**
* **Grid Search**

### Parâmetros Analisados
Os principais hiperparâmetros ajustados durante os experimentos foram:
* `n_estimators`: Quantidade de árvores no conjunto.
* `max_features`: Limite de características consideradas em cada divisão de nó.
* `max_depth`: Profundidade máxima das árvores para controle de complexidade.
* `min_samples_split`: Amostras mínimas necessárias para a divisão de um nó.

## Resultados

* **Acurácia Inicial:** 88% (configuração padrão).
* **Desafio Encontrado:** Durante os testes iniciais de otimização, os resultados oscilaram entre 80% e 82% devido ao desbalanceamento da base de dados.
* **Resultado Final:** Após ajustes específicos nos parâmetros para lidar com os dados, alcançou-se uma acurácia de **89%**.

## Conclusão
O estudo demonstrou que o Random Forest apresenta um desempenho nativo elevado para este dataset. Embora as técnicas de otimização tenham proporcionado um ganho marginal (de 88% para 89%), o processo validou a importância do tratamento da base de dados em conjunto com o ajuste fino de hiperparâmetros.

---
**Autores:** Fábio Carvalho e Sara Pacheco  
**Instituição:** IDP - Engenharia de Software (3º Semestre)
# Experimento de Equidade em Software (*Software Fairness*)

Este projeto foi desenvolvido com o objetivo de replicar e aplicar a metodologia científica apresentada no artigo **"Ignorance and Prejudice" in Software Fairness (ICSE 2021)**. 

O foco da experiência é avaliar como o tamanho do conjunto de *features* (conhecimento do modelo) e o nível de viés de representação nos dados de treino (preconceito) afetam simultaneamente a acurácia e a equidade de um modelo de *Machine Learning* aplicado à deteção de fraudes financeiras.

## Contexto da Experiência

* **Bases de Dados:** 10 conjuntos de dados sintéticos gerados com diferentes níveis de viés de representação.
* **Modelo Utilizado:** Árvore de Decisão (*DecisionTreeClassifier*).
* **Atributo Protegido:** `RAMO_ATIVIDADE`
  * Grupo Privilegiado: `1`
  * Grupo Desprivilegiado: `4`
* **Métricas de Avaliação (via IBM AIF360):** * Acurácia
  * *Statistical Parity Difference* (Paridade Estatística)
  * *Average Abs Odds Difference*
  * *Equal Opportunity Difference*
  * *Disparate Impact*

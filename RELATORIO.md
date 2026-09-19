Problema e Dataset escolhido:

Diabetes é uma doença que afeta muitos indivíduos ao redor do mundo, e há a necessidade de saber os hábitos e as possíveis causas dessa doença, para que um indivíduo saudável possa evitar desenvolvê-la.
O dataset escolhido foi o CDC Diabetes Health Indicators, um estudo feito com o objetivo de relacionar estilo de vida com diabetes.


Pré-processamento realizado:

As etapas do pré-processamento foram: verificar valores faltando, remover o público de 65 anos para cima do dataframe, remover duplicatas.


Perguntas e respostas da análise exploratória:

1. Há alguma relação entre diabetes e pressão alta?
R: Sim, há uma clara relação entre pressão alta e diabetes, vendo que a maioria dos diabéticos tem pressão alta, e a maioria dos não diabéticos tem pressão normal.

2. Existe alguma relação entre IMC (BMI) e diabetes?
R: Sim, vendo que o IMC de quem é diabético é, em média, 5 a mais de quem não é diabético.

3. Fazer exercício físico ajuda a prevenir diabetes?
R: Não foi encontrada relação entre a prática de exercícios físicos e a prevenção de diabetes.

4. Fumar aumenta as chances de alguém desenvolver diabetes?
R: Não foi encontrada relação entre o fumo e o desenvolvimento de diabetes.

5. Há alguma relação entre idade avançada e diabetes?
R: Foi analisado que os grupos mais velhos sempre têm mais casos de diabetes do que os grupos mais jovens.


Modelos treinados e comparação de métricas:

Foi treinado um modelo de regressão logística, um modelo de árvore de decisão, e um modelo Random Forest. A acurácia dos modelos ficou acima de 0.8, e foi observado que a classe 0 tem notas altas de precisão e recall, ficando com um f1 de 0.9 ou acima nos três modelos. No entanto, o f1 da classe 1 não superou 0.44 em nenhum modelo. Isso mostra que os modelos não são bons em prever casos de diabetes baseado nos dados do dataset. Pode-se concluir que boa parte das variáveis de estilo de vida não são boas para diagnosticar um caso de diabetes, apesar das relações encontradas.




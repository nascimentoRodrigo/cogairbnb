# cogairbnb
Classificação do room type (feature ‘room_type’) da base de dados da Airbnb disponível no link (“http://insideairbnb.com/get-the-data.html”)

a)	Como foi a definição da sua estratégia de modelagem?
a.	A estratégia utilizada foi identificar os tipos de dados que existia dentro da base de dados, em seguida excluir colunas e linhas de dados vazios para não influenciar de forma negativa os modelos finais. Como por exemplo a coluna “neighbourhood_group” é uma coluna totalmente vazia então há excluímos. Posteriormente categorizei toda a coluna “neighbourhood” de forma binária e assim tivemos uma informação mais completa, e um modelo classificatório mais robusto. Para que isso seja validado verificamos a correlação entre os dados para que pudessem assim ser confirmada as informações selecionadas.

b)	Como foi definida a função de custo utilizada?

c)	Qual foi o critério utilizado na seleção do modelo final?
a.	Foi construído um algoritmo com 7(sete) modelos, tais modelos foram classificados como; Classificadores simples e outro como ensemble, pois dependendo do classificador poderíamos ter um modelo bom, em seguida selecionamos o modelo que apresentou uma acurácia maior entre os modelos, em nosso caso o classificador/modelo “Random Florest”.

d)	Qual foi o critério utilizado para validação do modelo? Por que escolheu utilizar este método?
a.	Existem diversas estratégias para validação do modelo a que escolhe foi do tipo “folder”, na qual dividi os testes em 10 partições de forma aleatória, dessa forma evitar viés positivo para qualquer modelo. Em seguida calculamos a acurácia do modelo de acordo com as informações imputadas no modelo, por exemplo: Os testes estavam divididos em 10 partes, para cada teste o algoritmo seleciona 1 das 10 partes de forma aleatória para o teste do modelo e quando finaliza o teste com as 10 partes obtivemos o resultado da acurácia.

e)	Quais evidências você possui de que seu modelo é suficientemente bom?
a.	O modelo “Random Florest” selecionado é bom, pois mineramos as informações contidas na base de dados bruta, e em seguida selecionamos somente as informações necessárias para realizamos o treinamento de vários modelos com técnicas diferentes e avaliá-los. Dessa forma temos um modelo robusto e bastante específico para classificar o “room_type”.

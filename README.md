# Mineração de Regras de Associação do Dataset SAGE
_Refinamento e busca de padrões para desenvolvimento de experiências gamificadas_

Para o primeiro trabalho da disciplina de Inteligência Computacional, devemos selecionar um dataset público para mineração de dados resultando na coleta de regras de associação.

O dataset utilizado foi publicado através de uma pesquisa com o intuito de ampliar a base de dados ligadas a jogos gamificados com o propósito de analisar as preferências de usuários e como enchergam diversas características ligadas ao game design.

## Link para publicação
[SAGE: A dataset for Smart Adaptive Gamified Education](https://sol.sbc.org.br/index.php/sbie/article/view/26738/26557)

O [dataset original](https://github.com/ArmandoToda/Paper_SBIE2023) pode ser encontrado no repositório do autor no github.

> Essa documentação também está disponível no [documento jupyter](SAGEMining.ipynb)

## Metodologia
Criei o repositório e arquivo jupyter para executar as etapas de mineração necessárias para busca de regras de associação:
- Definição de variáveis para operação do projeto
- Obtenção do dataset
- Preparação dos dados
- Filtro de Canônicos (opcional)
- Binarização de dataset
- Execução do algoritmo apriori

## Resultados
Para uma melhor compreensão dos agrupamentos de dados e sua relevância, decidi fazer um plotting das associações obtidas com base nos eixos X,Y,Z representando os valores de Confidence, Lift e Certainty.

Com um suporte mínimo de 0.3 e confiança mínima de 0.7, mais de 500 resultados foram encontrados.
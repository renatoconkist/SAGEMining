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
Com um suporte mínimo de 0.3 e confiança mínima de 0.7, mais de 500 resultados foram encontrados.
Classificações que passam no suporte mínimo
- gender_male, gender_female
- age_group_15-24, age_group_25-34
- country_us
- years_playing_10-20
- time_per_week_<5, time_per_week_5-15
- game_genre_role playing game
- setting_multiplayer_False, setting_multiplayer_True

Para uma melhor compreensão dos agrupamentos de dados e sua relevância, decidi fazer um plotting das associações obtidas com base nos eixos X,Y representando os valores de Confidence e Certainty com coloração de Lift.

Nos resultados podemos observar uma forte presença de atributos como progressão e objetivo. Isso reflete diretamente em boa parte das associações apresentadas.
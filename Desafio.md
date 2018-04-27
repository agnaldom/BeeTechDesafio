# Desafio BeeTech

## Pontos importantes:

* Orientação a objetos
* Arquitetura/Design interno da aplicação
* Clareza e organização do codigo
* ECMAScript 6

Extras:

* Interface gráfica bem acabada
* Uso avançado da linguagem e/ou framework

Caso se sinta limitado(a) pelo tamanho do projeto, fique a vontade de estender um
pouco os requisitos. O teste deverá ser feito usando JavaScritp, ou seja, o backend deverá ser
construído usando Node.js e no front, se possível, utilize React, caso não se sinta confortável
com esta biblioteca, sinta-se livre para escolher algum outro framework. Pode ser utilizado
qualquer biblioteca externa, principalemnte para os testes (Mocha, Jest, jasmine...).

## Desafio

A empresa de telefonia BeePhonica, especializada em chamadas de longa distância 
nacional, vai colocar um novo produto no mecardo chamado FaleMais. Normalmente um
cliente BeePhonica pode fazer uma chamada de uma cidade para outra pagando uma tarifa
fixa por minuto, com o preço sendo pré-definido em uma lista com os códigos DDDs de 
origem e destino:

|Origem  |Destino  |$/min  |
|--------|---------|-------|
|011     |016      |1.90   |
|016     |011      |2.90   |
|011     |017      |1.70   |
|017     |011      |2.70   |
|011     |118      |0.90   |
|018     |011      |1.90   |

Com o novo produto FaleMais da BeePhonica o cliente adquire um plano e pode falar de
graça  até um determinado tempo (em minutos) e só paga os minutos excedentes. Os minutos
excedentes tem um acrescimo de 10% sobre a tarifa normal do minuto. Os planos são
FaleMais 30 (30 minutos), FaleMais 60 (60 minutos) e FaleMais 120 (120 minutos).

A BeePhonica, preocupada com a transparência junto aos seus clientes, quer
disponibilizar uma página na web, onde o clinete pode calcular o valor da ligação. Ali, o cliente
pode escolher qual o plano FaleMais. O sistema deve mostrar dois valores: (1) o valor da ligação com
o plano e (2) sem o plano. O custo inicial de aquisição do plano deve ser desconsiderado para este problema.

Caso o DDD do cliente não esteja presente na listagem de DDDs, a BeePhonica gostaria
de capturar os dados desses clientes (DDD, nome e email) para entender quais regiões
possuem maior demanda e consequentemente notificá-los quando tais regiões estiverem disponíveis.

Ex: 

|  Origem  |  Destino  |  Tempo  | Plano Fale Mais | Com Fala Mais | Sem Fala Mais |
|----------|-----------|---------|-----------------|---------------|---------------|
|011       |016        |20       | FaleMais 30     | $ 0,00        | $ 38,00       |
|011       |017        |80       | FaleMais 60     | $ 37,40       | $ 136,00      |    
|018       |011        |200      | FaleMais 120    | $ 167,20      | $ 380,00      |
|018       |017        |100      | FaleMais 30     | -             | -             |

Para fazer o deplou da aplicação poderá ser utilizado algum servidor gratuito, para que 
não seja gerado custos, como AWS ou a heroku.
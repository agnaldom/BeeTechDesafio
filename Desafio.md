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
|--------|---------|-------|

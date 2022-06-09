# Como trabalham as três formas de declarar varieavies em Javascript Var, Let e Const

## Scopo
O que é Scope?
Existem dois tipos de escopos, o local e o global. No Javascript cada função gera um escopo, ele é responsavel por determinar acesso ou visibilidade de uma variavel. As variaveis definidas dentro da função não são acessiveis ou visiveis fora dessa função. 

Scope Chain é a capacidade de uma variel ser declarada dentro de um escopo de função buscar seu valor até chagar no escopo global.

O que delimita um escopo de uma variavel do tipo "var" é a função.


## Redeclaração
A variável do tipo "var" aceita ser redecladado varias vezes, retornando o ultimo valor declado.

A variavel do tipo "let" só permite ser redeclado dentro do bloco que foi declado. Não sendo preciso o seu tipo na declaração.

No "const" o tipo de variavel não aceitar ser redeclado em momento algum.

## Hoisting
Capacidade do codigo resgatar o valor de uma declaração antes da sua inicialização.

O "let" não ceita ser declarado depois da sua inicilização. Informando erro.
# Explicando como funciona o Babel

O Babel é um transpilador de codigo javascript que conver o código para uma versão entendivel por todos os navegadores.

A ideia do surgimento do Babel se da pelo fato das varias atialização e mudanças criadas pela ECMA, com sua versões ES6 e demais. Com base no Traceur, trasnpilador criado pelo Google, e com junção de algumas bibliotecas como Escodegen, Esprima e o Estraverse.

O Babel transpila ou transcompila o codigo javascript em um codigo que seja compativel conm todos navegadores. O babel permite executar os melhores e mais atuais recursos da linguagem com o melhor desenpenho mesmo que o navegadfor nem seja compativel.

### Para que o Babel faça a transpilação do Codigo ele executa 3 passos:

Parser - transforma o codigo(AST) para uma Abstract Syntax Tree(AST) que é uma estrutura de dados
onde todos os elementos do codio js são mapeados.

Transformer - manipula os dados estruturados da forma que achar melhor(codigo AST)

Generator - Tranforma o codigo(AST) em outro codigo js

O Babel é utilizados em diversas outras ferramentas como
Bundles: Webpack, Grunt, Gult, Browserify
Frameworks: Ember, Rails
Ferramentas de Teste: Jasmine, Ava, Mocha
Libs: .Net, Node, Ruby

Sendo compativeis com as extenções .js, .jsx, .ts, .tsx.

E usado pelo Google, Spotify, Apple, Netflix.



Baixar babel
configurar babel.config.js

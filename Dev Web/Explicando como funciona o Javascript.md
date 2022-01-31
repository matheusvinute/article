# Explicando Javascript

Javascript é um codinome para a implementação do ECMAscript, ela é hoje uma das linguagens de programação mais utilizadas no mundo e mesmo os que não gostam muito dela acabam tendo que aprender e codar.

Você agora provavelmente deve esta em algum navegador ou algum app desenvolvido com algum framework desenvolvido em Javascript. Não tem jeito Javascript é onipresente e estará entre nós por muitos anos ainda.

ECMA é o acronimo de European Computer Manufacture's Association, pelo nome parace ser uma associação só da Europa, mas na verdade é uma organização global. Inclusive passou a se chamar ECMA International justamente para refletir isso. Essa organização tem uma importancia gigante pra todos os consumidores de tecnologia, ela cria padrões de especificações de padrões de comunicação usando tecnologia. Exemplo:

Especificação ECMA-404: é referente a especificação do JSON

Especificação ECMA-408: é referente a especificação do Dart

Especificação ECMA-262: é referente a especificação do Javascript (que acabou se chamando de ECMAscript)

O ECMAscript é também uma especificação e não o Javascript em se, portanto o Dart jscript, também podem ser considerados especificações ECMAscript.

Quando falamos em ECMAscript acaba sendo referencia ao próprio Javascript, inclusive não tem nada haver com Java. Ele foi lançado em 1995, no Netscape 2.0, como o nome de Livescript. O que ninguém imaginava é que essa linguagem que só servia para validar formulários e fazer algumas coisisnhas com o DOM, fosse alcaçar voos tam altos.

Com um pouco de entendimento da história vamos enteder porque dos nome ES4,ES5 e ES6. Eles antes faziam essas especificações por edição, aliás o ES4 que é a quarta edição foi abandonada em 2003 e apartir da 6 edição, eles começaram a utilizar o ano, o ECMAscript 2015 era chamado anteriormente de ES6. Isso é importante saber pois agora temos edições de 2016 até 2022, ou seja, a cada ano a linguagem vai ganhando novas funcionalidades e corrigindo alguns problemas desde a época do Livescript.

Nós citamos o ECMAscript4 justamente por ter sido a tentativa de melhorar a linguagem desde a ultima atualização em 1999. Nessa época tentaram adicionar classes, sistemas de módulos, tipos estaticos, generators, mas foi completamete abandonado. Tentar mudar muitas coisas de uma vez só não deu certo e muitas dessas ideia só acabaram sendo incorporadas no ES6, que é considerado a edição com uma melhoria expressiva na liguagem.

Javascript é uma linguagem multi paradigma com recursos para orientação a objetos, mas tipagem fraca, ela também é uma linguagem dinâmica, ou seja, não é necessário definir os tipos das variáveis antes da compilação. Muitos programadores não curtem muito esse lançe de tipagem dinâmica, pois ela acaba dando margem para os problemas aconterem durante a execução. Isso não está totalmente errado, mas não podemos negar que o Javascript sendo dinâmico, é parte do sucesso da linguagem.

Para resolver esse guepe da linguagem a Microsoft criou o TypeScript, que é o supersete pro Javascript. Com o TypeScript é preciso definir a tipagem, tendo também mais controle dos objetos. Com o TypeScript a sensação é de estar lidando com o paradigma da Orientação a Objetos, mas no fim tudo vira Javascript pra ser interpretado pelo motor JS. Por falar em motor podemos falar no SpiderMonkey (desenvolvido na Mozila e utilizado pelo Firefox), JavaScriptCore (criado pela Apple e utilizado no Safari), V8Engine (foi criado pelo Google e é a base do Google Chrome), que foi responsável por levar o Javascript para o BackEnd, também utilisando o Node.js e mais recentimente pelo Deno que são "run times" que permite levar a execução do Javacript para outras plataformas fora do navegador, criados pela mesma pessoa Ryan Dahl.

Ryan Dahl é um dev americano de apenas 40 anos que mudou a forma como se usa Javascript no mundo. O Nodejs foi o run time que conseguil essa façanha e é hoje muito presente nos computadores dos desenvolvedores, ele surgiu com o conceito de Javascript Every Where e cumpre fielmente seu papel. Node pode não só ser visto no back end de aplicações web mas também é possivel rodar Javascript em dispositivos IoT, por exemplo. 

Quando foi lançado em 2009 o Node deu uma sacudida total na comunidade Javascript e foi um dos responsáveis junto com o jQuery por colocar o Javascript novamente no mapa e isso era o que faltava para apartir de 2011 começar uma série de melhorias na linguagem, não podemos esquecer que ainda exitem devs mais puristas que não reconhecem Javascript como uma linguagem de programação de verdade.

Um pouco de código:

-Básico de JS

<button onclick="alert('olá mundo!')">Click Aqui</button>

-Usando o recurso Destructuring(ES6), podemos chamar de desestruturação, essa é uma expressão que permite descompactar valores de arrays ou propriedades de objetos em variáveis distintas, algo muito útil, nesse exemplo ao invéz de criar-mos uma atribuição para cada item do array, fazemos isso em uma atribuição somente.

const casal = ["Gabriel", "Vanessa"];

// Sem destructuring

const gabriel = casal[0];

const vanessa = casal[1];

// Com destructuring

const [gabriel, vanessa] = casal;

console.log(gabriel);

console.log(vanessa);

// Destructuring mais bem elaborado;

const perfil = {

nome: "Vanessa",

idade: 59,

altura: 1.49,

graduacao: "Ciência da Computaçao",

pos_graduacao: "gestão Empresarial",

profissao: "Programadora",

estado_civil: "casada"

};

const {nome, idade, altura, graduacao, pos_graduacao, profissao, estado_civil, } = perfil;

console.log(nome);

console.log(idade);

console.log(estado_civil);

console.log(profissao);

Outra grande mudança no ES6 foi a introdução de módulos e isso ajudou muito em libs e frameworks como React, Styled Components, Next.js, Vue.js e outros.

-Os Módulos tornam possível criar códigos como funções e classes ou até mesmo variáveis que podem até mesmo ser importado em outros arquivos e isso permitiu dividir ainda mais as funcionalidades. Exemplo, abaixo:

// melhor_canal.js

const melhorCanalDePorgramacao = () => "Código Fonte TV";

export { melhorCanalDeProgramacao as melhorCanalSemHumildade }; 

// meu_app.js

import { melhorCanalSemHumildade } from "./melhor_canal.js";

console.log(melhorCanalSemHumildade()); // Código Fonte TV

Outro recurso é a Promises, que é a capacidade de executar scripts em uma trade em background da trade principal da aplicação, isso veio da implementação das web works e permitiu que o código rodace sem nenhum tipo de bloqueio ou atraso. Com as Promises é simplesmente maravilhoso e necessário(código Assícrono).

Desestruturação, Rest, Modulos, Promises(callback e async/await) 

-----------------------------------------------------------------------------------------------------

## Desafio de Entendimento JS

### Escopo

No Javascript exitem dois tipos de escopo: Escopo Local e Escopo de Global. No Javascript cada função cria um escopo.

Escopo define a visibilidade(acessibilidade) de uma variavel.

Variáveis definidas dentro de uma função não são visíveis fora da função.

Exemplo:

var nome = 'Matheus vinute';

console.log(nome);

O resultado é a string armazenada na variavel "nome". Tanto a variável nome quanto o comando "console.log", eles estão no mesmo escopo, que é o global.

O Javascript trabalha com o conceito de Scope Chain, que define como que o acesso as variaveis são propagadas dentro do JS. Quando voce declara uma variavel em um escopo os escopos internos conseguem acessar esses valores, independente da profundidade interna.

Exemplo:

var nome = "Matheus Vinute";

function retornarNome(){

return nome;

}

retornnarNome();

Note que na função "retornarNome" não possui nenhuma variavel definindo nome e por conta do Scope Chain a função busca no escopo acima o valor da variavel nome.

### Qual a diferença entre usar "var", "let" ou "const"

Deve ser levado em consideração 3 coisas quando o assunto é declaração de variavel no JS, que são: 1-Escopo, 2-Redeclaração e 3-Hoisting.

1-Escopo - O que delimita o escopo de uma variavel tipo var é a função, ela não consegue estrapolar o limite imposto por uma função.

Exemplo de como funciona:

function alguem(){

var nome = 'Matheus';

return nome;

}

console.log(nome); // erro, com o nome não definido, já que a variavel esta delimidade pela função.

alguem(); // certo, retorna o nome declarado na variavel dentro do escopo da função

Então a primeira característica do var é ter Function Scope(Função de Alcance).

2-Redeclaração - Uma variavel de tipo var aceita ser reedeclarada normalmente. Um exemplo disso:

var nome = "Matheus";

var nome = "Bernardo";

console.log(nome); // o resultado vai ser sempre o ultimo valor repassado a variavel

OU

var nome = 'Matheus';

function alguem(){

nome = 'Ribeiro';

return nome;

}

alguem(); // vai retornar o valor do nome atribuido, limitado ao escopo da função

console.log(nome); // vai erro(nome is not defiened), isso que dizer que variavel sofreu uma mudança de seu valor, limitada somente a ao escopo, se tornando indefinida. 

3-Hoisting - Significa levantar algo para cima(içar algo), o interpretador de JS antes de executar o código, faz isso para todas as variáveis do tipo var e todas as declarações de funções. Quando é declarado um var nome na parte de baixo do código, antes de executar qualquer coisa, ele move esse var para o topo do escopo. E mantida a atribuição do valor dentro da variavel não alterando seu valor, mas ele eleva a declaração para o topo.

Exemplo:

console.log(nome); // erro, porque a variavel nome não esta definida

var nome;

console.log(nome); // indefinido, porque a variavel foi declarada, mas seu valor não foi definido

console.log(nome);

var nome = 'Matheus Vinute'; // indefinido, pois ele identificou a variavel mas não seu valor

var nome;

console.log(nome);

nome = 'Matheus Vinute';

console.log(nome) // 'Matheus Vinute', e declarado a variavel, comando de exibição no meio e a atribuição do seu valor por ultimo, executando o recurso hoisting, retornando dois valores undefined e 'Matheus Vinute'.

"Sempre declare variáveis no topo de código."

-Funcionamento do Hoisting pro Let e Const

Let é um tipo de declaração de variavel do tipo Let Scope, ou seja, essa variável só é permitido seu uso no escopo declarado, esse recurso é usado quando as variaveis foram criado destro de condicionais ou loops não deixem vestígios para outras partes do codigo que pode representar um comportamento inesperado.

A Redeclaração no Let acontece depois de uma vez declarada, ela deixa o valor ser alterado. Exemplo:

let nome = 'Matheus';

nome = 'Vinute';

console.log(nome); // Vinute, recebe o ultimo valor tedno o let nome já declarado

O Hoisting no Let, ele também esta sujeito a esse recurso elas não são inicializadas com o valor undefined(indefinido), logo, é necessario declará na forma correta para não haver erro. Exemplo:

console.log(nome);

let nome = 'Matheus Vinute'; // Erro, nome não foi definido

Const lembra muito o funcionamento do Let possuindo também o Escopo de Bloco, Sofre Hoisting mas não é inicializado e não pode ser redeclarado, mas diferente do Let o valor não pode ser nem retribuído. Se uma Const apontar para algum valor ele vai ficar apontando pra la sempre, não sendo possível ser reapontado para outro valor.

Exemplo:

const nome =  'Matheus';

nome = 'Vinute';

console.log(nome) // Erro, pois o Const não aceito reatribuição de valor

Qual a diferença entre os dois exemplos a seguir sobre a criação de uma função?

function myFunc(){

​	// alguma logica

}

and

var myFunc = function(){

 //alguma logica

}

No primeiro exemplo é criado uma função Work Function direto e no segundo caso é declarado uma variavel myFunc e depois uma função é atribuida nessa variavel. Suas diferenças, a primeira diz que a função pode ser iniciada no inicio do script no segundo script somente depois da inicialização. Isso quer dixer que existem duas formas de registrar funções no javascript, uma é o Function Declaration e o outro é o Function Expression.

Function Declaration é como no primeiro exemplo do desafio, voce declara ela com a Key Work Function, a partir de momento que voce declara ela dessa forma ela vai esta disponivel independete da ordem do seu script. Exemplo:

teseDeclaration();

function testeDeclaration(){

console.log('Testando Function Declaration');

}

// Resultado Testando Function Declaration

Function Expression, ela possui esse nome pois fica do lado da expressão. Exemplo:

testeExpression();

var testeExpression = function() {

console.log('Testando Function Expressions');

}

// E retornado uma Erro dixendo que o testeExpression não é uma função


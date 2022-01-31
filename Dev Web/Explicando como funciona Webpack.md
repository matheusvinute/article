# Webpack

O Webpack esta ligado a área de desenvolvimento front end ele é um Bundle, ou seja um agrupado/empacotado de arquivo Javascript. A utilização de um agrupador se torna muito útil quando estamos utilizando a programação modular, que consiste em programar cada funcionalidade de forma separada, em outras palavras, é dividir um problemas em pequenas partes menores.

Dividir a aplicação em módulos tem algumas vantagens incluindo a facilidade de resolução de debugs e teste, já que cada um desses módulos deve ter o seu propósito bem definido no contexto geral da aplicação.

O Webpack é quem faz a junção de tudo isso(módulos), o Webpack faz o gerenciamento das dependencias desses módulos e apartir de um arquivo inicial ele cria um Dependency Graph, traduzindo uma Arvore de Dependencia, e é atravez dessa arvore que ele deixa toda desorganização dos módulos organizado. 

Para um melhor entendimento da relevancia de um Dependency Graph no uso de uma aplicação é muito comum que um módulo dependa um do outro para executar alguma funcionalidade. Você não poderá instanciar um determinado objeto em sua aplicação se o módulo que o criava ainda não foi chamado. Quando  se trata de projetos pequenos que não possui muitos módulos é facil organizar e controla os módulos, mas quando é muito grande tendo vários desenvolvedores ai se faz o uso de um gerenciador de dependia, o Webpack.

O Webpack ele varre os arquivos, verifica e resolve as dependências através do Dependency Graph, gerando no final um Bundle, um pacode arquivos js, pronto para ser utilizado.

O Webpack surgiu ... , nessa época existiam duas formas de utilização do JS. A primeira contendo um script para cada funcionalidade e a segunda gerando um arquivo JS gigante, contando todo o seu código. Depois surgiu o Immediately Invoked Function Expression, ou IIFE, resolve o problema dos projeto maiores e é nesse contexto que se encaixa as ferramentas como o Gulp e Grunt. Essas são as   Task Runners, essas ferramentas facilitam bastante o desenvolvimento, pois é com elas que é possivel organizar o projeto em arquivos separados e no final gerar um arquivo só, disponivel para produção.

Muitas pessoas confudem o Webpack com um Task Runner, mas ela vai alem dessas funcionalidades, podendo ser suadas em conjunto. Com o sugimento dos módulos (Modules), muito em influencia do V8Engine, que possibilitou que o Javascript saisse do navegador e podesse ser utilizado em outros ambientes como em um servidor e até em banco de dados. E isso possibilitou que o Javascript entrasse em uma nova era.

Com isso veio um problema sobre onde vão ser carregados os código se não há mais necessidade do HTML/CSS e das tags de scripts? Com isso surgiu o CommonJS com o require que permite o carregamento e a utilização dos módulos em um arquivo. Solucionou um dos lados pois ele é bom pra utilização com NodeJS, mas ai passou a ser o navegador que não suporta o CommonJS. Surgiram outras ferramentas para fazer com que o navegador entendesse o CommenJS como Browserify e o RequireJS. O ECMAScript Modules esta trabalhando no ESM para resolver esse guep nos navegadores, enquanto isso o Webpack preenche bem essa vaga.

Ele se tornou a melhor ferramenta para fazer Bundle das aplicações JS, sem falar que da suporte para o CommonJS quanto ao ECMAScript Modules e ainda pode ser estendido para dar suporte a imagens CSS e Fonts.

O Webpack funciona como pacote do Node.JS e fará sua instalação atravez do npm, em bora não seja obrigadorio o Webpack utiliza um arquivo de programação que voce poderar customizar diversas partes da sua utilização. Esse arquivo é o webpack.config.js, se ele não existir o Webpack utilizará todas as suas configurações no modo default. Para a criação desse arquivo customizado é importante entender alguns conceitos como o 

Entry, que é o ponto de partida para a construção da arvore de dependencias, ela pode ser definida com a Single Entry(string), Object Syntax(objeto) ou Multi Page Application(multipla aplicação).

Output, que indica o caminho de saida do Bundle criado.

Loaders, que ajudam ao Webpack a processar outros tipos de arquivo e cnvertelos para modulos que possam ser consumidos na aplicação, incluindo na arvore de depencias.

O Webpack só consegui entender fora do ambiente dois tipos de arquivo o Javascript e o Json, dendo dois atributos o teste e o use.
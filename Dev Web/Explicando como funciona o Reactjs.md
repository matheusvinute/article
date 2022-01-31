O React foi criado pelo Engenheiro do Facebook Jordan Walker, no principio foi chamado de FaxJSV e era utilizado apenas internamente nos projetos da propria empresa como o Facebook e no Instagram. Na JsConfUS em 2013 ja com o nome de React o projeto foi anunciado como open source, desde então o React é uma das principais ferramentas de desenvolvimento Front-End.

Em resumo o React é declarativo e eficiente. Ele permite compor UIs completos de pequenos e isolados códigos, os chamados Componentes. Ele também é flexível, ou seja, é possível utilizar React em uma pequenas parte do site com algumas linhas de código e nenhuma ferramenta de Build, ou em projetos mais completos, como na criação de um Sigle-Page App nesse caso sim utilizando de algumas outras ferramentas que facilitam e agilizam o trabalho dos desenvolvedores com essa lib.

Para o setup básico de uma aplicação React é necessário a importação de duas bibliotecas o React DOM (que faz a ligação entre o React e os elementos da pagina, o DOM) e o React em se, que contem as funcionalidades principais como a criação de elementos, manipulação de estados, hooks entre outras funcionalidade que fazem o React ser o que é.

Entre os vários arquivos e componentes do React, ele possui um arquivo chamado Babel, que é um compilador de javascript. Ele permite que seja utilizadas funcionalidades modernas da linguagem que podem ainda não ser suportado por todos os navegadores.

Pra explicar mais o funcionamento do Babel e uma das principais características do React, temos que falar do Virtual DOM. Manipular o DOM pode ser muito custoso para o funcionamento da aplicação, para resolver isso o React possui o Virtual DOM, que é uma representação das informações dos elementos do DOM que ficam salvos na memória. O React mantem uma cópia virtual de todas as informações do DOM, quando uma mudança é detectada, invés de renderizar todo o DOM o React consegui identificar na sua cópia virtual qual o elemento terá suas informações atualizadas, para assim renderizar o seu equivalente no DOM.

Essa característica faz com que o Reat tenha uma excelente performance ao renderizar mudanças no DOM. 

Mas como passamos as informações dos elementos que queremos criar no React? A resposta é com Javascript. 

A criação de elementos no React é feito através de funções Javascript da propria biblioteca.

Para que utilização da biblioteca não fique uma bagunça com excesso de comandos em Javascript, o React possui uma linguagem de marcação chamada de JSX.

O JSX que significa Javascript XML, permite uma sintaxe similar ao HTML no momento da criação de elementos para o React deixando esse processo muito mais amigável.

O Babel por sua vez vai por traz das cortinas, transforma a sintaxe do JSX em funções Javascript.

O uso do JSX é não obrigatório no React, mas por conta de sua familiaridade com o HTML podendo usar Javascript ele passa a ser uma boa opções de escrita das funcionalidades da aplicação. 

Assim como o Vue e Angular a Componentização é um dos principais pilares na utilização do React para dividir suas aplicações em partes independentes, isolados e reutilizadas. Um componente pode ser representado por uma simples função Javascript desde que ele atenda dois requisitos.

1-Aceitar um parametro de propriedade, as Props.

2-Retornar um React Element, que é o JSX

Qual a diferença da criação de Componente por Função e por Classe?

Antes da versão 16.8, a criação usando Função possui restrições, como por exemplo, sem Estado e Hooks. Apartir dessa versão as funcionalidades foram adicionadas aos Componentes. Sendo assim, o método de desenvolvimento do componente vai muito a gosto de desenvolvedor.

React é um biblioteca que pode precisar de outras bibliotecas para adicionar algumas funcionalidade extras. Uma das mais utilizadas é o 

1-Redux, que é uma lib para o gerenciamento de Estados, uma aplicação com vários componentes trocando informações entre se acaba se tornando bem dificil de gerenciar e o Redux centraliza todo de forma bem eficiente.

2-React Router, é uma lib para lidar com as Rotas de uma aplicação

3-React Intl, disponibiliza varios componentes para manusear datas e numeros.

Outro item importante é o React DevTools, uma extenção do Google Chrome com diversas ferramentas de debug para aplicações em React.
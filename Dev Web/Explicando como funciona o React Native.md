# O que é o React Native ::atom_symbol:

React Native é um framework javascript para criação de aplicações nativas para dispositivos mobile, ele é um projeto open source e mantido pelo Facebook. Desde seu lançamento em 2015 o React Native já conquistou a confiança de milhares de desenvolvedores no mundo contando até com grande empresas.

Não dá para falar do React Netive sem antes falar do React. O React ja é bem conhecido pelos desenvolvedores e mesmo assim tem quem confunda as duas soluções.

O React é uma biblioteca javascript para construir interfaces que tem como conceito principal a utilização de Componentes, ela também é open source e mantida pelo Facebook.

O React Native utiliza o React para nativamente Renderizar aplicações Android e IOS, em outras palavras, o React funciona exatamente como na web só que em vez de renderizar o HTML no React Natice ele renderiza os Componentes Mobile para cada uma das paltaformas.

Com o conceito de Learn once, write anywhere, o React Native possibilita a criação de apps para Android e IOS com a mesma base de código sem nenhuma ou quase nenhuma alteração do código. Por exemplo em 2015 a equipe do Facebook divulgou que o aplicativo Facebook Ads Maneger possuia 87% do mesmo codigo base entre o Android e IOS, ja no Discord 98% do código é compartilhado entre as suas diferentes versões.

Os Componentes são utilizados no React Native através da marcação JSX, que se assemelha um pouco com o XML. O próprio framework possui por padrão varios componentes prontos para o uso além de deixar o desenvolvedor livre para criar quantos mais ele quiser, por exemplo, botões, listas, formularios, alertas, imagem e muitos mais.

Internamente o React Native faz uma chamada para as API's nativas da plataforma Andoid ou IOS para renderizar esses componentes o que faz os apps terem sua aparece e usabilidade totalmente nativas, em outras palavras, esse trabalho pesado de utilizar as API's em Java no Android e Swift em IOS ficam por conto de React Native. E o resultado são Componentes totalmente nativos diferente das web views que são HTML Renderizado e que são uma solução para apps chamdos hibridos.

Além disso o React Native também permite a utilização das API's de cada plataforma atravez do javascript , isso quer dizer que será possível utilizar as funcionalidade do proprio dispositivo como a camera, telefone, localização e outros. Tudo com javascript.

Quanto ao suporte, atualmente o framework é compativel com Android e IOS, o que nos faz pensar que ele se limita a penas a duas plataformas, mas ele tambem tem sua versão para Computador também React Native Desktop, Windows e macOs. Graças a sua comunidade ativa.

Quando comparamos como outros framework o React Native fica em vantagem com relação as tecnoligias chamada hibridas, que utilizam o HTML e são apresentados atravez de Web Views, que é uma especie de navegador dentro do aplicativo, que vem alguns pontos negativos, quando se utiliza um web view não se usa nativamente as funcionalidades da plataforma sendo necessario autilização de plugins que agem entre o web view e a plataforma , isso vem com um custo de performance e alem disso a usabilidade é baseada em uma recriação do HTML, CSS e JS de forma nativa, ou seja alem de afetar a performance a aparência também não exatamente as melhores. Ja o React Native traduz suas marcações JSX para elementos completamente nativos utilizado as API's internas da plataforma, promovendo uma experiencia completemanete nativa e em altíssima performance.

Além disso o React trabalha em uma camada separa das API's de rederização e isso significa que ele pode manter a alta performance sem sacrificar as funcionalidade do React Native.

## Componente, Propriedades e Estado

Componentes permitem você devidir a UI em partes independentes, reutilizáveis, ou seja, trata cada parte da aplicação como um bloco isolado, livre de outras dependências externas. Os componentes são como funções Javascript. São partes isoladas que tem estilos e comportamento em um bloco isolado que podem ser reaporveitados em todo o projeto. Componentes podem ser escritos em forma de função e classes.

Propriedades são chamados de "props", ele retorna elementos que descrevem o que cada componente deve aparecer na tela. São valores que podem ser passado a um componente para que ele utilize esse valor. São estaticas.

Estado não é repassado ao componente e sim configurado dentro dele. Pense no estado como as propriedades de nossa classe que devem ser armazenadas para renderizarmos o componente da forma correta. O estado não é repassado ao componente e sim configurado dentro dele.São Mutáveis.Estados são como variaveis por exemplo o nome. Sua sintaxe const[nome, setNome] = useState('Matheus'), o 'nome' comunica onde no codico deverar passar o valor 'Matheus'(useState), já o setNome passa a mudança criado aparti de outra função, por exemplo: 

function entrar(){

setNome('Sujeito Proramado')

}

## Var, Let e Const

Var - define uma variavel que pode ser definida e utilisado no escopo e fora do escopo no aplicativo.

Let - deficini uma variavel que so pode ser acessada dentro do escopo no codigo do aplicativo.

Const - é definido no codigo e não pode ser alterada, é um valor fixo.

## Flexbox

O Flexbox foi projetado para fornecer um layout consistente em diferentes tamanhos de tela. Assim como temos na web no React Native functiona da mesma forma.

au se utilizar o Flexbox, é preciso ter em mente que todas as operações realizadas relacionam-se ao eixos: o eixoprincipal(Main Axis) e o eixo transversal(Cross Axis).

O eixo principal é definido através da propriedade fex-direction e o eixo transversal encontra-se na direção perpendicular a ele.

A propriedade flex-direction define a direção do eixo principal e pode ter quatro valores possíveis:

1. row
2. row-reverse
3. columm
4. column-reverse

Podemos utilizar proporções com a propriedade flex para ocuparmos o tamanho conforme o peso estabelecido para cada objeto(container).

# Conhecendo a estrutura Inicial

-Pasta tests, para criação de teste automatizados

-Pastas android e ios, onde é copilado para o modo nativo

-Pasta node_models, contem as dependências do objeto

-git, pata trablah com git

-prattierrc.js, deixa o codigo mais organizado 

-watchmanconfig, que recebe as auterações e repaça ao emulado

app.json, onde vai permitir na fase final dar nome e descrição, logo do app

index.js, ponto de entrada onde a aplicação vai começar

metro.config, onde acontece a compilação

package.json, onde ficam as dependencias de desenvolvimento, scripts
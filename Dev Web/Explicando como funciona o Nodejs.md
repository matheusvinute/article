Node é um ambiente para a execução de código Javascript, ou seja, ele empacota tudo que é necessário para executar e interpretar códigos em Javascript. Em outras palavras, da mesma forma que nós conseguimos executar código Javascript em nosso navegador, com Node é possível executar em um ambiente fora dele, abrindo um mundo de possibilidade de utilização para a linguagem.

Hoje em dia o Node se propagou tanto que você pode esta utilizando ele e nem sabe. Utilitários como o Grunt, Gulp, Webpack, NPM são desenvolvidos em Node e costumam esta no dia a dia de milhares de programadores. A utilização do Node é mais comum em Aplicações Web, porem sua utilização pode ir além, é possível a utilização de utilitários de linha de comando conhecidos como CLI, aplicações desktop, chatbots e tem até gente criando redes neurais com Node.

Essa vasta possibilidade de utilização do Node se deve a utilização do motor V8 do Google, o V8 também conhecida como Maquina Virtual V8 é o motor de interpretação Javascript, desenvolvido pelo Google e que é usado no navegador Chrome e em diversos outros como o Opera. Ele é responsável por compilar o código Javascript pro formato nativo de máquina antes de executa-lo, acelerando seu desempenho fazendo ele ser executado na velocidade de um código binário. E foi por conta dele que o Javascript deixou de ser uma linguagem utilizado apenas no insight e passou a fazer parte do Back-End de um site, em aplicações de rede e scripts de utilitários. 

Mas a estrela principal pela popularização do Node se dá pela utilização do Javascript porque possui desde seu nascimento uma arquitetura não bloqueante baseada em eventos, que merece um grande destaque por se diferenciar das demais tecnologias utilizadas antes de sua popularização. A arquitetura do Javascript é dividida em basicamente em três partes: 

Call Stack - responsável por empilhar as chamadas de funções;

Callback Queue - que é responsável por empilhar os Callbacks das funções, passadas por essas funções assíncronas;

Event Loop - que é responsável continuamente por fazer a checagem se algum evento assíncrono foi disparado executando assim sua respectiva Callback;

Para ilustrar como o Node funciona vamos dar o exemplo de restaurante:

Quando um cliente novo chega no restaurante o garçom vai até a mesa anotar o pedido do cliente, após isso o pedido é levado até a cozinha e o cliente fica aguardando seu pedido. Enquanto isso o garçom continua trabalhando atendendo os pedidos dos novos clientes, assim que um pedido é finalizado o garçom se dirige até a cozinha para levar o pedido até o cliente. Repetindo isso continuamente.

Esse exemplo representa uma Arquitetura não-bloqueante de thread única, ou single thread.

Agora associando esse exemplo em uma aplicação web vemos que:

Substituindo o restaurante por uma Aplicação Web que devolvera uma informação simples de um banco de dados. O garçom é a thread única, os cliente são os usuários e a cozinha representa os processos de negócio. Quando o usuário acessa o site o back end precisa processar as regras de negócios como de acessar o banco de dados e devolver o resultado. Nesse caso chamaremos uma Função Assíncrona passando uma Call Back com o que queremos que aconteça quando esse processamento terminar, a Call Back ficará no no Call Backs Queue ou seja será executado posteriormente quando o processamento da função assincrona for finalizado. Assim que o processamento da função assincrona for finalizado um evento será disparado. O Event Loop, que fica sempre atento aos eventos que ocorrem, identifica esse evento colocando nossa função de Call Back no Call Stack, ou seja, na fila das funções a serem executadas.

Após isso nossa função é executada devolvendo pro usuario o resultado esperado.  Essa Arquitetura foi feita para não travar a execução, enquanto a regra de negócio é processada mesmo quando uma requisição é feita o usuario continua livre para interagir com a aplicação enquanto ele espera a resposta do processamento, deixando a experiencia do usuário muito mais fluida.

Mas qual seria a Arquitetura das Linguagens Convencionais Multithread? Linguagem como o PHP, Ruby, Asp.net não possuem esse comportamento de thread única não bloqueante, ou seja, eles não conseguem atender mais de uma requisição por vez, forçando o usuário a esperar caso esteja executando outra requisição.

Seguindo o mesmo exemplo do Garçom no Restaurante, imagine que ao inves do garçom atender outra mesa, após levar o pedido do cliente para a cozinha ele fique parado esperando o pedido do cliente ficar pronto, para só então levar ao cliente que pedio e depois ir atender outra pessoa. Ou seja, o garçom fica com tempo ocioso, parado esperando o pedido ficar pronto.

As linguagens tradicionais são multithread, ou seja, a cada requisição ele cria uma nova thread, se o servidor chegar no limite de thread simutaneas, ou seja, tiver muitos acessos ao mesmo tempo os usuários teram que aguardar até que uma thread termine para abrir espaço para uma nova thread, nesse caso para evitar um gargalo de acesso é necessário adquirir mais servidores, que gera mais custos.

Assim como tudo na tecnologia no Node não é a solução para todos os problemas, a arquitetura baseada em eventos no Javascript torna o Node ideal para aplicações com IO inteços, ou seja, entrada e saida de dados intenço. Exemplos como chat, stream, servidores web, comunicação de redes em geram já que sua especialidade é servir mais usuarios utilizando menos hardware e no fim se transforma em mais performance com menos gasto. O Node não é recomendado para aplicações que utilizam alto uso da CPU, como a manipulação de videos, imagens. Pois isso exige uma grande quantidade de calculo demandando esforço maior da CPU.

Com o Modelo Single Thread do Node ao realizar esses calculos a thread ficaria completamente parada até obter o resultado final dessas operações fazendo as requisições não atendidas ficarem em modo de espera tornando nossas aplicações bloqueantes. Isso acabaria com o propósito de estarmos utilizando não bloqueante e não queremos isso. Então nesse caso é melhor evitar a utilização do Node.

Diversas empresas adotaram o Node como tecnologia, exemplo:

Paypal, Uber, Netflix, Walmart.
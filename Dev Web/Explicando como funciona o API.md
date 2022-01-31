API é a sigla para Aplication Program Interface. Ela pode ser empregada em qualquer contexto de desenvolvimento de software. Uma definição clara sobre uma API é que se uma interface de um sistema é criada para que um usuario final possa usa-la a API é desenvolvido para que um sistema possa usar as funcionalidade de um sistema de outro sistema programaticamente. Ou seja, a API é a interface ideal para que um sistema se comunique com outro sistema, compartilhando suas ações, ferramentas, padrões e protocolos.

Ao conectar os sistemas as APIs tem um papel essencial na criação de aplicativos, os aplicativos que conhecemos hoje só são possiveis apartir de ligação entre diversos sistemas e ferramentas.

Exemplo de Caso de Uso:

Mercado Livre - atravez das APIs abriu muitas possibilidades para outros sistemas se integrarem com suas ferramentas, abrindo caminho para que grandes varejistas podessem usar a plataforma cadastrando produto, gerindo estoque, administrando agendas, pagamentos entre outros.

As APIs não necessariamente precisam trabalhar via web, muito se fala em API Rest, usando HTTP, mas a verdade é que o conceito de API pode estar presente em qualquer tipo de sistema inclusive no sistema operacional. O Windows possui internamente internamente as API prontas para seus desenvolvedores criarem seus softwares integrados com suas funcionalidades do sistema operacional permitindo criar sistema de arquivo, permissão, dispositivos entre outros.

API Rest é uma API como qualquer outra, porém utilizando o protocolo HTTP mais especificamente a versão 1.1. Quando navegamos na web estamos usando 99% dos casos HTTP, que é um protocolo de comunicação e esse tipo de protocolo aceita alguns tipos de métodos o GET, POST e HEAD isso possibilita acessar paginas, enviar formulários. A API Rest aceita ainda o PUT, DELETE, TRACE, CONNECT. E com esses novos metodos é possivel criar APIs bem melhores e padronizadas.

EndPoints, essa palavra é muito utilizada no mundo das APIs e muita gente confunde achando que um EndPoint é algum tipo de API. O EndPoint é a extremidade de um canal de comunicação, isso seria representado como uma URL do servidor. O EndPoint é o que o serviço expõe e ele tem três caracteristicas conhecidas como ABC. A - ADDRESS, onde o serviço esta hospedado. B -BINDING, que é como o serviço pode ser acessado. C - CONTRACT, que é o que pode ser visto no serviço. 

Um exemplo de serviço de EndPoints é o GoogleCloudEndPoint, com ele é possivel implantar, proteger, monitorar, analisar e também veicular suas API com a mesma infra estrutura usada pelo Google nas suas proprias APIs. E possivel usar qualquer linguagem ou biblioteca para escrever uma API e adicionar uma especificação, OpenAPI ou configuração com o gRPC API, e o GoogleCloudEndPoint fará o monitoramento e a proteção de sua API

Segurança nas APIs, elas usam o SSL para toda a solicitação e os dados enviados  pelas APIs serão transportados criptografados usando protocolo HTTPs, mas a segurança na comunicação não é o unico aspecto a ser levado em conta na API. Ainda temos a autenticação, que serve para isolar o que pode ser fornecido de informação para cada um dos softwares que chama a API, afinal ningem vai querer  consultar dados sensiveis que so podem ser utilizados pelos seus respectivos donos e para isso se utilizam muitas tecnicas de autenticação, mas sem duvida a mais utilizada pelos desenvolvedores é a geração de Tokens. Os Tokens são amplamente utilizados nas APIs e geralmente são identificadores unicos que nada mais são do que uma sequencia aleatorio de caracteres e são enviados juntos das chamadas aos EndPoints das APIs. Os Tokens são chaves que ficam guardados e são validados exatamente como se fossem uma senha, só que apartir dai os dados podem ser liberados para acesso. Esse tipo de autenticação é tao poderosa que pensa-se ate em abolir as senhas tradicionais, por que não se consideram tam seguras assim no processo de autenticação.

Retorno, que tipo de informação uma API volta e como é possivel que um sistema consome essa API , possa manipular essas informações. Quando falamos de API, não necessariamente estamos falando de API para a web, então o tipo de informação é inerente a cada API. o que acontece é que na web esses formatos via padronização deles é bem disseminado. Estamos falando do uso do JSON ou XML, esses dois formatos são utilizados para retornar os dados da APIs baseadas em web. 

Exemplos de APIs

GetSongBPM - serve para dizer quantas batidas por minuto tem uma musica 

Google

Youtube 

Paypal - sistema financeiro 
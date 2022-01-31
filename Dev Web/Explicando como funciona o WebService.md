Web Services são soluções para aplicações se comunicarem independente de linguagem, software e hardware utilizados.

Inicialmente Web Services foram criados para troca de mensagens utilizando a linguagem XML(Extensible Markup Language ) sobre o protocolo HTTP sendo identificado por URI(Uniform Resource Identifier)

Podemos dizer que Web Services são  APIs que se comunicam por meio de redes sobre o protocolo HTTP

Para um exemplo de uso de APIs vamos a um exemplo:

Uma empresa X tem uma aplicação no Servidor X e BD X e Uma empresa Y com sua aplicação no Servidor Y e BD Y. Digamos que a empresa Y queira acessar o BD da empresa X de forma segura usa-se o Web Service, que vai expor por meio de uma URI, que vai fazer troca de mensagens por meio de XML ou JSON. Permitindo assim que sistemas de linguagens diferentes e com o acesso seguro a a dados.

Vantagens de utilizar um Web Service

-Linguagem comum

-Integração

-Reutilização de implementação

-Segurança

-Custos

Principais tecnologias

-SOAP, Simple Objetect Access Protocol, é um protocolo baseado em XML para acessar serviços web, principalmente por HTTP. Pode-se dizer que SOAP é uma definição de como serviços que se comunicam. Foi desenvolvido para facilitar integrações entre aplicações.

Vantagens, permite integração entre aplicações, independente de liguagem, pois usa como linguagem comum o XML, é independente de plataforma e software, meio de transporte genérico, ou seja, pode ser usado por outros protocolos alem do HTTP.

Partes do SOAP

1-SOAP Envelope: é o pricipal elemento do documento e é usado para encapsular toda a mensagem SOAP

2-SOAP Header: é o elemento onde possui informações de atributos e metadados da requisição(IP de oridem, DNS, Token)

3-SOAP Body: é o elemente que contem os detalhes da mensagem(ordem do que fazer a aplicação, conteudo)

-REST, Representational State Transfer, é um estilo de arquitetura de software que define a implementação de um serviço web. Pode trabalhar com XML, JSON e outros.

Vantagens do REST

-Permite integração entre aplicações e tambem entre clientes e servidor em paginas web e aplicações. Utiliza dos metodos HTTP para definir a operação que esta sendo efetuada. Arquitetura de facil compreensão.

Funcionamento do REST

Cliente faz uma requisição HTTP(GET,POST, PUT, DELETE) e o servidor responde um codigo de operação(retorna mensagem texto, JSON, XML)

-XML

-JSON, Javascript object notation, formatação leve utilizada para troca de mensagens entre sistemas. Usa-se de uma  estrutura de chave e valor e tambem de listas ordenadas. Um dos formatos mais populares e mais utilizados para a troca de mensagens entre sistemas.


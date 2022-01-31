## Deploy

Deploy, traduzindo para o português significa implantar, colocar em posição, disponibilizar para uso, ou ainda, colocar no ar. Essa palavra é muito utilizado no meio dos desenvolvedores, tendo diversas formas de se fazer um deploy evoluiram muito nos ultimos anos.

Subir para o servidor o site que foi desenvolvido que estava só na sua maquina, pode ser considerado um deploy, ou quando você gera uma nova versão de um programa e quer implantar ele em servidor de aplicação, que pode ser um ambiente de homologação ou produção tambem significa fazer um deploy.

Existe diferença entre implantar e implementar, possui significado diferente.

Atualmente extem três forma de se fazer Deploy.

1- Manual: Um exemplo disso é o FTP, para uso de modificações pequenas.

2- Parcialmente Atualizado: Pode ser o PUSH no branch master, que é feito no repositório Git, que roda um Hook e atualiza o servidor de hospedagem. A vantagem tipo de Deploy é o controle de versão e o histórico de cada Deploy. 

3- Completamente Automatizado: É o que ha de mais moderno no desenvolvimento de sistemas, ele esta intimamente ligado com o conceito de automatização continua. Além da cópia o Deploy continuo traz vantagens de se trabalhar com diversas alterações, tambem conhecidas como integrações feito por diversos programadores. A ferramenta de Deploy, nesse caso, faz todos os testes necessários para que não haja problema em juntar todas integrações em produção, sue uso, atualizar bibliotecas, testar conectividade de servidores, similar visitas e entrada de dados. Tudo de forma automatica e se algo der errado  o Deploy é revertido. 

Jenkins é umas das ferramentas mais utilizados para fazer Deploy automatizado, ele garante um alto nivel de produtividade, segurança e qualidade no desenvolvimento de software.
# Como funciona os Bancos de Dados Não Relacional

NoSQL ou Not Only SQL é um tipo de banco de dados não relacional. O NoSQL não descarta completamente a utilização do SQL, ele esta relacionado a área de DataBase e ao desenvolvimento de Sistemas como grande volume de armazenamento e pesquisa de dados.

**Qual a diferença de Banco de Dados Relacional para um Não Relacional?**

O Banco de Dados Relacional são baseados em esquemas, ou seja, é preciso primeiro projetar uma estrutura criando tabelas, campos e relacionamentos entre elas pra depois conseguir adicionar algum dados.

O Banco de Dados Não Relacional os esquemas não são necessários.

NoSQL é apenas um banco de dados, existem muitas tecnologias e ferramentas que, para esse tipo de banco de dados. Existem 5 bancos de dados NoSQL sendo de Chave e Valor, Grafos, Colunas, Pesquisa e Documentos.

1-Chave e Valor: são muito utilizados em jogos, publicidade e internet das coisas. Eles são altamente particionáveis e permite escalabilidade horizontal. Ele armazena dados no padrão chave-valor. Exemplos MemcacheD, Riak, Redis.

2-Grafos: organizam os dados na forma de grafos utilizando vértices e arestas, sua principal função esta na criação de aplicativos que precisam de um conjunto de dados altamente conectado. Seu pricipal uso esta nas Redes Sociais, Detecção de Fraude, Nos mecanismos de reconhecimento e criação de gráficos de conhecimento. Exemplo Property Graph RDF, ferramentas para gerenciamento de banco de dados é o Neo4j e o Giraph.

3-Colunar: tambem conhecido como orientado a colunas, que é um tipo que armazenas dados em linha particulares de tabelas no disco. O banco de dados Colunar é utilizado para recuperação rapida de colunas de dados. O armazenamento orientado a colunas para tabelas com banco de dados é um fator ultra importante para a performance de consulta analitica, pois ele reduz expressivamente a entrada e saida em disco, diminuindo a quantidade de dados que voce precisa carregar no disco. Exemplo: Cassandra e Hbase.

4-Pesquisa: é um modela especificamente construido para indexação, agregação e pesquisa de dados semi estruturados. Esse modelo é pensado na performance, baixa latência e  analise de dados em tempo real. Exemplo: Amazon ES, Expedia.

5-Documento: armazena os dados em documentos, ele tambem é conhecido como modelo de dados semi estruturados. Um documento que pode ser definido criando uma estrutura complexa de dados com proprio formato chave e valor, utilizando o formato JSON. Documentos se tornam unidades independentes o que faz uma melhor performance da leitura de dados, tornando mais fácil distribuir dados em multiplos servidores. Exemplo MongoDB, CouchDB.

**Motivos para usar Banco de Dados NoSQL**

1-Flexibilidade: No mundo cada vez mais ágil, onde a prática de desenvolvimento ágil é um padrão no mercado, trabalhar em projetos onde a estrutura de dados é intuitiva e flexivel, é um dos motivos para se adotar. Por que as praticas de desenvolvimento ágil, preconizam entregas rápidas e contínuos do projeto onde a complexidade para mudanças precisam se baixas e o nível de adaptação alto.

2-Escalabilidade: os Banco NoSQL são pensados exatamente na escabilidade horizontal, ou seja, distribuindo dados usando clusters ao invés dos joins. Dessa forma quando o voluma de dados e tambem a quantidade de usuários aptos a sua-los possam crescer sem gargalos. 

3-Disponibilidade: quando um banco de dados ficam indisponivel, dependendo do nivel critico do sistema pode representar de dinheiro e de clientes. Por isso a maior parte dos banco de dados NoSQL oferecem arquiteturas muito "parrudas" de replicação de dados clusterização, o que torna a disponibilidade ainda maior que os outros modelos. A clusterização permite que toda vez que um nó caia a outro que poderá assumir automaticamente e sem perda de dados.

4-Open Source: os banco de dados NoSQL tem seu código fonte aberto, o que permite seu crescimento rápido e melhorias continuas. Exemplos de banco de dados Cassandra e CouchDB, que é mantido pela Apach foundation e o DynamoDB mantido pela Amazon.

5-Infraestrutura e Custo: o custo para iniciar e migrar para um banco de dados NoSQL é muito baixo e o simples fato de ser open source ajuda nisso. Os bancos de dados relacionais precisam de server com o poder de processamento e hardware mais avançados do que os banco de dados NoSQL, isso representa mais custos. Como o NoSQL ja foi pensado desde seu inicio para trabalhar em ambientes distribuidos isso acaba somando ainda mais em favor dele.

6-Recursos Especiais: suporte a banco de dados API Restfull, alguns oferencem replicação automatica, sincronização, capacidade de consulta, entre outros
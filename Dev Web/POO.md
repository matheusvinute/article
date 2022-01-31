# Paradigma da Orientação a Objetos ::man_technologist:

**O que é** Paradigma de programação de computadores  onde se usam **classes e objetos**, criados a partir de modelos usados para **representar e processar dados**.

A programação Orientada a Objetos organiza o software em pequenas partes ou objetos distintos que são responsáveis por manipular uma estrutura de dados por meio de características e ações predefinidas. Nessa metodologia, **comportamento e estrutura** de dados estão muito relacionados, diferentemente das antigas tecnologias estruturais em que isso não era possível. 

O paradigma da Orientação a Objetos é fundamentado por quatro características:

**Abstração** a abstração esta relacionada à definição precisa de um objeto. Esta definição inclui sua identidade(nome), suas características(ou propriedades) e o conjunto de ações que ele desempenha. Tomemos como exemplo um cachorro: o objeto cachorro deve ser único e não poderá ser repetido. Neste ponto o objeto já tem identidade definida. Sua característica se dá pela cor do pelo, peso, raça, e por ai vai. Por fim, as ações que ele é capaz de desempenhar incluem latir, fareja, pular etc. Definimos o objeto cachorro .

**Herança** é a característica que permite o objeto filho herdará características e comportamentos do objeto pai. Vamos a um exemplo:

Gerente:arrow_right:Funcionário 

Podemos ilustrar a herança com os dados do modelo "Funcionário". Eles devem identifica-lo, por exemplo, como o nome, cargo e data de admissão. No exemplo, existe uma categoria especial de funcionário chamado "Gerente" que, além desses dados, deverá também conter a quantidade de funcionários que gerencia e a senha de acesso ao sistema da empresa.

O modelo "Gerente" herda características do modelo "Funcionário", especificamente os dados Nome, Cargo e Data de Admissão. Esta é a ideia central da herança: aproveitar características e comportamentos gerais em modelos mais específicos. Esta particularidade nos permite entender que um objeto mais abaixo é um caso especifico do objeto acima, ou seja, ele possui as características gerais do objeto pai, acrescidas de mais algumas especificidades que o diferem do seu ancestral.

**Polimorfismo** Consiste em dar outra forma à alguma ação herdade do objeto pai.  Vamos a um exemplo:

Imagine um eletrodoméstico qualquer. Uma de suas ações consistem em ligar. No entanto, os objetos forno de micro-ondas e televisão, que são especializações de eletrodomésticos, são ligados de forma diferentes. Por isso, para cada um dos objetos filho, a ação ligar será descrita de modo diferente.

O Polimorfismo permite que classes diferentes sejam tratadas de mesma forma, sendo compreendida como a capacidade de um objeto ser referenciado de varias formas.

**Encapsulamento** pode ser entendida como uma técnica utilizada para limitar o acesso às variáveis (atributos), aos métodos, ou até mesmo, às próprias classes, escondendo os membros da classe(atributos e métodos) e tornando o sistema mais suscetível a mudanças.

Uma vez que o objeto é Encapsulado, seus detalhes de implementação, não são mais imediatamente acessíveis. Ao invés disso, eles empacotam e são somente indiretamente acessíveis através da interface do objeto. A única forma de acessar a um objeto encapsulado é através da troca de mensagem: enviando uma mensagem ao objeto, o objeto mesmo seleciona o método pelo qual ele irá reagir a mensagem.

## Classes e Objetos

**Classe** descreve os objetos, com seus atributos, métodos que servem para sua construção.

**Objeto** serão um individuo extraído, ou produzido pela sua fábrica, a classe. Dentro da filosofia de desenvolvimento orientado a objetos, nosso objetivo primário sempre será a escrita das classes, e então, a utilização dos objetos para a execução de uma tarefa.

Hooks são recursos do Reactjs, responsavel por executar uma
funcionalidade especifica. Sua identificação se dá pelo uso
dos use...

useState - hook que armazena informação. Sua estrutura é composta
por um: 
const [], array que possui dois indices o primeiro uma variavel
segundo uma função que altera a variavel(estado inicial)
useState(), que possui o valor inicial.

useEffect - hook responsvael por executar o ciclo de vida de um
codigo em determinada circusntancia. Possui dois parametros:
() => {} - uma arrow function que executa uma função,
[] - variavel, que compara o que esta sendo executado

useContext - hook para repasse de dados que são mais complexas ou
que seu repasse indpenda de elevação de dados, independa de acesso
de um componente superior.

Suas partes de concionamento são:

1- .Provider, . Consumer

2- Arquivo de criação de contexto
import {createContext} from 'react';

export const TransactionContext = createContext();

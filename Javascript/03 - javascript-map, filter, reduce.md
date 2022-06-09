## map

Um objeto Map itera seus elementos na order da inserção - um loop for...of retorna um array de [key, value] para cada iteração.

Em outras palavras é uma função responsavel por transformar os elementos de array, tendo seu aray resultante o mesmo tamanho do array original, sendo necessario uma função para transforma os elementos iterados. Sendo possivel chamo valrias vezes em seguido transformando os dados trabalhos.

## filter

filter() chama a função callback fornecida, uma vez para cada elemento do array, e constrói um novo array com todos os valores para os quais o callback retornou o valor true ou  um valor que seja convertido para true. O callback é chamado apenas para índices do array que possuem valores atribuídos; Ele não é invocado para índices que foram excluídos ou para aqueles que não tiveram valor atribuído. Elementos do array que não passaram no teste do callback são simplesmente ignorados, e não são incluídos no novo array.
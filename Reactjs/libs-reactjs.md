## Axios 🕸️

lib que faz a interceptação de requisições e resposta, criando uma regra quando for feito uma requisição antes de chegar no backend da aplicação, como token de autenticação ou informação especifica ou em resposta, para fazer logout de acasso.

Vantagens de usar o Axios:

1-Encurtamento de link de acesso, com o axios a parte base do link, fuca aguarado dem uarquivo exclusivo, permitindo que seja usado a base com uma rota espeficica na parte do código que vá ser trabalhado.

2-Adaptação para json, com axios o retorno do servidor já vem formando em json, graças ao axios.

## Styled Components 🖊️

1-Suporte encadeamento de stylos, como como sass.

2-Estiliza o componente utilizando o javascript aplicando somente no componente em especifico sua propriedades.

## Miragejs 🔃

Permite criar uma API Fake dentro do nosso Front End. Suas vantagens:

1- Tem Banco de dados integrandos

2- Relationships

3- Permite configurações que simulam um backend de serviço propriamente dito

4- Pode ser executado em paralelo ao funcionamento do Front End

### Explo de Código

`
import {createServer} from 'miragejs';

createServer({
  routes(){
    this.namespace = "api";

    this.get('/transactions', () => {
      return [
        {
          id: 1,
          title: "Transação 1",
          amount: 400,
          category: "Food",
          createdAt: new Date()
        }
      ]
    })
  }
})
`

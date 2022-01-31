# Principais verbos http



Os verbos http correspondem uma parte importante da "interface uniforme" restringe e fornece a ação para acesso a um determina recurso de uma aplicação. Os principais verbos http são GET, POST, PUT, PATCH, DELETE. Eles correspondem a criação, leitura, atualização e deleção criando assim a operação CRUD. Existem inúmeros outros verbos mas esses são os mais utilizados.

| HTTP Verb | CRUD           | Status Interno          | Item Especifico               |
| --------- | -------------- | ----------------------- | ----------------------------- |
| POST      | Create         | 201(Create)             | 404(Not Found), 409(Conflict) |
| GET       | Read           | 200(Ok)                 | 200(Ok), 404(Not Found)       |
| PUT       | Update/Replate | 405(Method Not Allowed) | 200(Ok) ou 204(No Content)    |
| PATCH     | Update/Modify  | 405(Method Not Allowed) | 200(Ok) ou 204(No Content)    |
| DELETE    | Delete         | 405(Method Not Allowed) | 200(Ok) 404(Not Found)        |



## Tipo de Parâmetros

Existem três tipo de parâmetros dois deles utilizados no método get e um no método post

- Route params
- Query params
- Body params

### Route params

Recebe nos dados da requisição na rota. Busca, atualiza e deleta. 

route params = /user/1

---

server.get("/user/:id", (req, res) => {

const{id} = req.params;

return res.json({message: `Buscando usuario com o ${id}`})

})



### Query params

Recebe os dados da requisição como parâmetro na URL. fazer consulta na aplicação.

Query params = ?name=Matheus

---

server.get("user", (req, res) => {

const name = req.query.name;

return res.json({message: `Hello ${name}`})

})

### Body params

Recebe os dados da requisição no corpo da requisição, geralmente me objeto na forma de JSON. Sempre utilizado no método POST da requisição.

{

"name": "Matheus", "idade": 15

}

---

server.post("/user", (req, res) {

const {name, idade} = req.body;

return res.json({id})

})

`POST /register -  FORMATO DA REQUISIÇÃO` </br>
`POST /signup -  FORMATO DA REQUISIÇÃO` </br>
`POST /users -  FORMATO DA REQUISIÇÃO`

```json
{
  "email": "xxxxx@xxxx.com",
  "password": "xxxxx",
 }
```

# json-server-base
Está api tem como objetivo, cadastrar comidas e tarefas.
## Endpoints -
A API tem um total de 7 endpoints, sendo que desses 7, 3 endpoints são utilizados para cadastro, 2 endpoints para login, 1 para o cadastro de comidas e 1 para o de tarefas.
### Criação do cadastro
`POST /register -  FORMATO DA REQUISIÇÃO` </br>
`POST /signup -  FORMATO DA REQUISIÇÃO` </br>
`POST /users -  FORMATO DA REQUISIÇÃO`
Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password. Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.
```json
{
  "email": "testinho@gmail.com",
  "password": "123456",
  "name": "Testinho",
  "age": 23
 }
```

### Para listar as comidas
```json
GET https://foods-tasks.herokuapp.com/foods
```

### Para listar as tarefas (precisa de autenticação)
```json
GET https://foods-tasks.herokuapp.com/tasks
```

### Para postar nos endpoints, foods e tasks precisam de autenticação
```json

Exemplo post foods

{
  "nome": "Hamburguer",
  "userId": 2
}

Exemplo post tasks

{
"descricao": "estudar.",
"userId": 2
}
``` 


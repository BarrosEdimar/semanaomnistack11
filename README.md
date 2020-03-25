# omniStack11

## Stack

1. Back-end: NodeJs + Express + SQLite
2. Front-end: React (JSX JavaScript XML)
3. Mobile: React Native + Expo

## Rota / Recurso

## Métodos HTTP:

1. GET: Buscar uma informação do back-end
2. POST: Criar uma informação no back-end
3. PUT: Alterar uma informação no back-end
4. DELETE: Deletar uma informação no back-end

## Tipos deparâmetros:

1. Query Params: Parâmetros nomeados enviados na rota apõs "?" (Filtros, paginação)
2. Route Params: Parâmetros utilizados para identificar recursos
3. Request Body: Corpo da requisição, utilizado para criar ou alterar recursos

```javascript 
  app.post('/teste/:id', (request, response) => {
    const params = request.params;
    const query = request.query;  
    const body = request.body;

    console.log(params, query, body);

    return response.json({ 
      evento: 'Semana OmniStack 11.0',
      aluno: 'Edimar Renato Santos Barros'
    });
  });
```

## DB

1. SQL: MySql, SQLite, PostgreSQL, Oracle, Microsoft SQL Serve
2. NoSQL: MongoDB, CouchDB, etc

1. Driver : SELECT * FROM users
2. Query Builder: table('users).select('*').where()

## Entidades

1. ONG
2. Caso (incident)

## Funcionalidade

1. Login de ONG
2. Cadastro de ONG
3. Logout de ONG
4. Cadastrar novo caso
5. Deletar cado
6. Listar casos especificos de uma ONG
7. Listar todos os casos
8. Entar em contato com uma ONG via WhatsApp e Email

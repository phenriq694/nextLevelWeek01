<h1 align="center">
  <img 
    alt="Nodejs" src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/1200px-Node.js_logo.svg.png" 
    width="200px"
  />
</h1>
<h2 align="center">
  Ecoleta API
</h2>


## Entidades:
- Points (Pontos de coleta);
- Items (Itens para coleta);

## Funcionalidades:
- Cadastro de um ponto de coleta;
- Cadastro de novos pontos de coleta;
- Listar pontos de coleta com base em localização;
- Listar informações de um ponto de coleta;
- Listar todos os tipos de itens;
 
## Rotas:
Para listar todas os itens:
```
GET '/items'
```
Para listar todos os pontos de coleta:
```
GET '/points'

Query Params:
{
  city: "",
  uf: "",
  items: "",
}
```
Para listar um ponto de coleta:
```
GET 'points/:id'
```
Para cadastrar um ponto de coleta:
```
POST '/points' 

Request Body
Multipart
{
  "name": "",
  "email": "",
  "whatsapp": "",
  "latitude": "",
  "longitude": "",
  "city": "",
  "uf": "",
  "items": ""
  "image": File
}
```

## Bibliotecas:
- typescript;
- express;
- knex;
- cors;
- celebrate;
- multer;

## Database:
- SQLite;

## Ferramentas:
- Insomnia;

## Como usar:

Para clonar essa aplicação, você precisará [Git](https://git-scm.com), [Node.js v10.16][nodejs] ou superior + [Yarn v1.21.1][yarn] ou superior instalado no seu computador. No seu terminal:

```bash
# Clone este repositório
$ git clone https://github.com/phenriq694/nextLevelWeek01.git

# Vá para este repositório
$ cd nextLevelWeek01/server

# Instale as dependências
$ yarn

# Execute as migrations
yarn knex:migrate

# Inicie a aplicação
$ yarn dev
```

[nodejs]: https://nodejs.org/
[yarn]: https://yarnpkg.com/
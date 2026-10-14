Você precisa completar um projeto de API CRUD em Node.js, incluindo clientes, pedidos e uma nova coleção de produtos. Vou te mostrar uma estrutura de exemplo que você pode adaptar ao repositório feito em aula.

## 1. O que precisa ser feito

- Clientes: concluir as operações de criar, listar, alterar e excluir.
- Pedidos: concluir as operações de criar, listar, alterar e excluir.
- Produtos: criar o arquivo `dados/produtos.json` e desenvolver todas as rotas CRUD.
- README.md: documentar as rotas e adicionar prints dos testes realizados no Thunder Client (extensão do VS Code).

## 2. Estrutura sugerida do projeto

text
```
projeto-api/
├── controllers/
│   ├── clientesController.js
│   ├── pedidosController.js
│   └── produtosController.js
├── dados/
│   ├── clientes.json
│   ├── pedidos.json
│   └── produtos.json
├── routes/
│   ├── clientesRoutes.js
│   ├── pedidosRoutes.js
│   └── produtosRoutes.js
├── app.js
├── package.json
└── README.md
```

## 3. Rotas CRUD que você deve implementar

| Método HTTP | Rota de exemplo | Operação |
| --- | --- | --- |
| GET | `/clientes` | Listar clientes |
| POST | `/clientes` | Cadastrar cliente |
| PUT | `/clientes/:id` | Alterar cliente |
| DELETE | `/clientes/:id` | Excluir cliente |
| GET | `/pedidos` | Listar pedidos |
| POST | `/pedidos` | Cadastrar pedido |
| PUT | `/pedidos/:id` | Alterar pedido |
| DELETE | `/pedidos/:id` | Excluir pedido |
| GET | `/produtos` | Listar produtos |
| POST | `/produtos` | Cadastrar produto |
| PUT | `/produtos/:id` | Alterar produto |
| DELETE | `/produtos/:id` | Excluir produto |

As rotas de consulta individual (`GET /:id`) também podem ser incluídas para completar o CRUD.

## 4. Exemplo de `dados/produtos.json`

json
```
[
  {
    "id": 1,
    "nome": "Teclado",
    "preco": 120.00,
    "quantidade": 10
  },
  {
    "id": 2,
    "nome": "Mouse",
    "preco": 65.00,
    "quantidade": 20
  }
]
```

## 5. Testes no Thunder Client

Faça testes de cada operação na sua API:

1. GET: verificar se os registros são retornados.
2. POST: cadastrar um novo registro usando JSON no corpo da requisição.
3. PUT: alterar um registro existente informando o ID na URL.
4. DELETE: excluir um registro existente e verificar o resultado.

Tire prints dos testes, salve-os em uma pasta como `prints/` e insira as imagens no `README.md`. Por exemplo:

markdown
```
## Testes da API

### Cadastro de produtos
![Teste POST de produtos](prints/produtos-post.png)

### Alteração de produtos
![Teste PUT de produtos](prints/produtos-put.png)

### Exclusão de produtos
![Teste DELETE de produtos](prints/produtos-delete.png)
```

Os nomes dos arquivos acima são exemplos: você deverá adicionar as capturas de tela reais dos seus testes.

## 6. Posso montar o código completo para você

Para desenvolver os controllers e as rotas corretamente, preciso saber como está o projeto que você utilizou em aula.

Você pode enviar o link do seu repositório do GitHub ou colar aqui o conteúdo do `app.js` e de um controller existente?

Assim, consigo seguir o padrão do seu projeto e preparar o código de clientes, pedidos e produtos, além de um `README.md` completo para você adaptar e publicar no GitHub.
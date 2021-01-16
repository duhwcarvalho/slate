# Paginação

> JSON:

```json
{
  "message": "Dados encontrado com sucesso!",
  "data": [
    {
      "name": "Terra",
      "size": "12.742 km"
    },
    {
      "name": "Marte",
      "size": "6.779 km"
    }
  ],
  "pagination": {
    "current_page": 1,
    "total_pages": 5,
    "per_page": 10
  }
}
```

<aside class="notice">
A API Wejam tem suporte a buscas em massa através dos métodos list. Todos esses métodos de listagem possuem uma estrutura em comum, que é a de <code>paginação</code>.
</aside>

**current_page** `number`

Página atual listada

**total_pages** `number`

Total de páginas possíveis para listagem

**per_page** `number`

Total de items listados na paginação atual

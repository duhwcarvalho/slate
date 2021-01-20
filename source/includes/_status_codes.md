# Status Codes
HTTP Status Codes

<aside class="notice">
A nossa API valida cada um dos campos enviados na requisição antes de prosseguir com a criação, consulta ou gerenciamento dos pedidos, transações e recursos.

Utilizamos os códigos de resposta convencionais do HTTP para indicar o sucesso ou a falha de uma requisição. Sendo assim, códigos <code>2xx</code> indicam sucesso, <code>4xx</code> indicam erros por algum dado informado incorretamente ou não encontrado (por exemplo, algum campo obrigatório não enviado ou um usuário não encontrado) e <code>5xx</code> indicando erros nos servidores da Wejam.
</aside>

> 200 - OK:

```json
{
  "message": "Usuário encontrado com sucesso.",
  "data": {
    "name": "Eduardo Carvalho",
    "email": "eduardo.wejam@gmail.com"
  }
}
```

> 400 - Bad Request:

```json
{
  "message": "Dado inválido.",
  "errors": "Definir um padrão aqui"
}
```

> 404 - Not Found:

```json
{
  "message": "Usuário não encontrado."
}
```

### Tabela dos HTTP Status Code


Código | Status | Definição
------ | ------ | ---------
200 | OK | Sucesso
400 | Bad Request | Requisição inválida
401 | Unauthorized | Chave(Token) de API inválida
404 | Not Found | O recurso solicitado não existe
412 | Precondition Failed | Parâmetros válidos mas a requisição falhou
422 | Not Acceptable | Parâmetros inválidos.
500 | Internal Server Error | Ocorreu um erro interno.
503 | Service Unavailable | Temporariamente offline para manutenção. Tente novamente mais tarde.

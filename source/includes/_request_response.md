# Solicitação/Resposta

> Exemplo de listagem vazia [404 - Not Found]

```json
{
  "message": "Nenhum dado encontrado.",
}
```

O formato de resposta padrão é JSON. As solicitações com um corpo de mensagem usam JSON simples para definir ou atualizar atributos de recursos.

**Algumas informações gerais sobre as respostas:**

<ul>
<li>IDs são retornados como inteiros.</li>
<li>Os campos em branco geralmente retornam <code>null</code> em vez de serem retornados como <code>strings</code> em branco ou <code>omitidos</code>.</li>
<li>Listagem vazia retorna status <code>404</code> em vez de <code>array</code> vazio.</li>
</ul>

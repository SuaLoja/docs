---
description: Documentação dos endpoints da tabela usuários.
---

# Usuários

{% api-method method="get" host="https://api.sualoja.app" path="/users" %}
{% api-method-summary %}
Consultar todos usuários
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="X-API-KEY" type="string" required=true %}
API KEY
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Usuários consultados com sucesso.
{% endapi-method-response-example-description %}

```
[
    {
        "id": "..."
        "firstName": "Victor",
        "lastName": "Guedes",
        "email": "victorfelipe.guedes@hotmail.com",
        "password": "..."
    }
    // ...
]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.sualoja.app" path="/users/:id" %}
{% api-method-summary %}
Consultar um usuário
{% endapi-method-summary %}

{% api-method-description %}
Consultar apenas um usuário com seu ID.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="ID" type="string" required=false %}
ID do usuário a ser consultado
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="X-API-KEY" type="string" required=true %}
API KEY
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Usuário consultado com sucesso.
{% endapi-method-response-example-description %}

```
{
    "id": "..."
    "firstName": "Victor",
    "lastName": "Guedes",
    "email": "victorfelipe.guedes@hotmail.com",
    "password": "..."
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Usuário com o ID consultado não encontrado.
{% endapi-method-response-example-description %}

```
{
    "status": 404,
    "message": "User not found",
    "error": "Not found"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}




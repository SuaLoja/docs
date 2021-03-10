# PATCH /users/:id/

{% api-method method="patch" host="https://api.sualoja.app" path="/users/:id" %}
{% api-method-summary %}
Atualizar apenas uma informação
{% endapi-method-summary %}

{% api-method-description %}
Atualizar email ou senha de um usuário.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="X-API-KEY" type="string" required=true %}
API KEY
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="email" type="string" required=false %}
Novo email do usuário
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=false %}
Nova senha do usuário
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Dados atualizados com sucesso.
{% endapi-method-response-example-description %}

```
{
    "id": "..."
    "firstName": "Victor",
    "lastName": "Guedes",
    "email": "{ new email },
    "password": "{ new password }"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Usuário não encontrado.
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


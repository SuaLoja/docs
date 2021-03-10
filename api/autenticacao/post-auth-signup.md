# POST /auth/signup

{% api-method method="post" host="https://api.sualoja.app" path="/auth/signup" %}
{% api-method-summary %}
Cadastrar um usuário
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

{% api-method-body-parameters %}
{% api-method-parameter name="firstName" type="string" required=true %}
Primeiro nome do usuário
{% endapi-method-parameter %}

{% api-method-parameter name="lastName" type="string" required=false %}
Último nome
{% endapi-method-parameter %}

{% api-method-parameter name="email" type="string" required=true %}
Email
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=true %}
Senha
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=201 %}
{% api-method-response-example-description %}
Usuário cadastrado com sucesso.
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
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}


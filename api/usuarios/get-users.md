# GET /users/

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


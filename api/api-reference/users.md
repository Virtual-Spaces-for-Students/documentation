# Users

{% swagger method="post" path="/users/login" baseUrl="http://localhost:3010" summary="Login" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" required="true" name="username" %}
email/pseudonyme de l'utilisateur
{% endswagger-parameter %}

{% swagger-parameter in="body" name="password" required="true" %}
mot de passe de l'utilisateur 
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Identifiant valides" %}
```javascript
{
    // Peut être le cookie
}
```
{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="Identifient invalides" %}

{% endswagger-response %}
{% endswagger %}


{% swagger method="get" path="/users/logout" baseUrl="http://localhost:3010" summary="Logout" %}
{% swagger-description %}

{% endswagger-description %}


{% swagger-response status="201: OK" description="" %}
{% endswagger-response %}

{% swagger-response status="403" description="" %}

{% endswagger-response %}
{% endswagger %}


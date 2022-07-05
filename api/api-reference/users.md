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

{% swagger-response status="204: No Content" description="" %}

{% endswagger-response %}

{% swagger-response status="403: Forbidden" description="" %}

{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/users/@me" baseUrl="http://localhost:3010" summary="Get User" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="patch" path="/users/@me" baseUrl="http://localhost:3010" summary="Modify User" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="query" name="password" %}
Ancien mot de passe
{% endswagger-parameter %}

{% swagger-parameter in="query" name="new_password" %}
Nouveau Mot de passe
{% endswagger-parameter %}

{% swagger-response status="204: No Content" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/users/@me/vms" baseUrl="http://localhost:3010" summary="Get User VMS" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response TBD
}
```
{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

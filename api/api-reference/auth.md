# 🔐 Auth

{% swagger method="get" path="/auth/login" baseUrl="http://172.18.8.2:8080" summary="Login" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="302: Found" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/auth/logout" baseUrl="http://172.18.8.2:8080" summary="Logout" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="204: No Content" description="" %}
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

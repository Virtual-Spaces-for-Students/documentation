# VM

{% swagger method="post" path="/vm" baseUrl="http://172.18.8.2:8080" summary="*WIP* Create Virtual Machine" %}
{% swagger-description %}

{% endswagger-description %}
{% endswagger %}

### Change d'état

{% swagger method="patch" path="/vm/{id}/start" baseUrl="http://172.18.8.2:8080" summary="*WIP* Démarrer la VM" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="204: No Content" description="Action effectué" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="VM introuvable" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

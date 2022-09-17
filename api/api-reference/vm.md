# VM

{% swagger method="post" path="/vm" baseUrl="http://172.18.8.2:8080" summary="*WIP* Create Virtual Machine" %}
{% swagger-description %}

{% endswagger-description %}
{% endswagger %}

## Change d'état

{% swagger method="patch" path="/vm/:id/start" baseUrl="http://172.18.8.2:8080" summary="*WIP* Démarrer la VM" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name=":id" required="true" %}
ID de la VM
{% endswagger-parameter %}

{% swagger-response status="204: No Content" description="Action effectué" %}

{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Déjà dans cet état" %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="VM introuvable" %}

{% endswagger-response %}
{% endswagger %}

{% swagger method="patch" path="/vm/:id/restart" baseUrl="http://172.18.8.2:8080" summary="*WIP* Redémarrer la VM" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name=":id" required="true" %}
ID de la VM
{% endswagger-parameter %}

{% swagger-response status="204: No Content" description="Action effectué" %}

{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Déjà dans cet état" %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="VM introuvable" %}

{% endswagger-response %}
{% endswagger %}

{% swagger method="patch" path="/vm/:id/stop" baseUrl="http://172.18.8.2:8080" summary="*WIP* Stopper la VM" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="query" name=":id" required="true" %}
ID de la VM
{% endswagger-parameter %}

{% swagger-response status="204: No Content" description="Action effectué" %}

{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Déjà dans cet état" %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="VM introuvable" %}

{% endswagger-response %}
{% endswagger %}

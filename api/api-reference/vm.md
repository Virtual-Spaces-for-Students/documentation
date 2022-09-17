# VM

{% swagger method="post" path="/vm/new" baseUrl="http://172.18.8.2:8080" summary="*WIP* Create Virtual Machine" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" name="name" required="true" %}
Nom de la VM
{% endswagger-parameter %}

{% swagger-parameter in="body" name="os" type="Integer" required="true" %}

{% endswagger-parameter %}

{% swagger-response status="201: Created" description="Crée" %}
```json
{
    id: ""// ID de la VM
}
```
{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Mauvaise configuration" %}

{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="Non connecté" %}

{% endswagger-response %}
{% endswagger %}

{% swagger method="delete" path="/vm/:id/delete" baseUrl="http://172.18.8.2:8080" summary="*WIP* Supprimer une VM" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="id" required="true" %}
ID de la VM
{% endswagger-parameter %}

{% swagger-response status="204: No Content" description="Supprimé" %}

{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="Non connecté" %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="VM Introuvable" %}

{% endswagger-response %}
{% endswagger %}

{% swagger method="patch" path="/vm/:id/start" baseUrl="http://172.18.8.2:8080" summary="*WIP* Démarrer la VM" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="id" required="true" %}
ID de la VM
{% endswagger-parameter %}

{% swagger-response status="204: No Content" description="Action effectué" %}

{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Déjà dans cet état" %}

{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="Non connecté" %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="VM introuvable" %}

{% endswagger-response %}
{% endswagger %}

{% swagger method="patch" path="/vm/:id/restart" baseUrl="http://172.18.8.2:8080" summary="*WIP* Redémarrer la VM" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="id" required="true" %}
ID de la VM
{% endswagger-parameter %}

{% swagger-response status="204: No Content" description="Action effectué" %}

{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Déjà dans cet état" %}

{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="Non connecté" %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="VM introuvable" %}

{% endswagger-response %}
{% endswagger %}

{% swagger method="patch" path="/vm/:id/stop" baseUrl="http://172.18.8.2:8080" summary="*WIP* Stopper la VM" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="query" name="id" required="true" %}
ID de la VM
{% endswagger-parameter %}

{% swagger-response status="204: No Content" description="Action effectué" %}

{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Déjà dans cet état" %}

{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="Non connecté" %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="VM introuvable" %}

{% endswagger-response %}
{% endswagger %}

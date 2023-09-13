---
description: Statistics API of instl
---

# Installation Statistics



{% swagger method="get" path="" baseUrl="https://instl.sh/api/v1/stats" summary="Installation count of all projects that use instl.sh" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200: OK" description="Installation count of all projects that use instl.sh" %}
```javascript
{
    "installer/instl-demo/windows": 1337,
    "installer/instl-demo/linux": 420, 
    "installer/instl-demo/macos": 1234
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/user/repo" baseUrl="https://instl.sh/api/v1/stats" summary="Installation count of specific project" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" required="true" name="user" type="String" %}
Owner of the GitHub repository
{% endswagger-parameter %}

{% swagger-parameter in="path" name="repo" required="true" type="String" %}
GitHub repository name
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Installation count per platform" %}
```javascript
{
    "linux": 3,
    "macos": 10,
    "windows": 15,
    "total": 28
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="" baseUrl="https://instl.sh/api/v1/stats/total" summary="Total count of installations handled by instl" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200: OK" description="Total installations" %}
```
1337
```
{% endswagger-response %}
{% endswagger %}

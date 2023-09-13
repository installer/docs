---
description: Badge API for shields.io support
---

# Shields.io Badge

{% hint style="info" %}
This API can be used with the [Endpoint Badge](https://shields.io/badges/endpoint-badge) of shields.io to create badges for your `README.md`
{% endhint %}

## Installation count of specific repository

{% swagger method="get" path="/user/repo" baseUrl="https://instl.sh/api/v1/badge/shields.io/stats" summary="Installation count badge" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="user" required="true" %}
Owner of the GitHub repository
{% endswagger-parameter %}

{% swagger-parameter in="path" name="repo" required="true" %}
Name of the GitHub repository
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Shields.io badge schema response" %}
```javascript
{
    "color":"orange",
    "label":"installations",
    "message":"4",
    "schemaVersion":1
}
```
{% endswagger-response %}
{% endswagger %}

## Total installations handled by instl&#x20;

{% swagger method="get" path="" baseUrl="https://instl.sh/api/v1/badge/shields.io/stats/total" summary="Total installations handled by instl badge" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200: OK" description="Shields.io badge schema response" %}
```javascript
{
    "color":"orange",
    "label":"handled installations",
    "message":"1337",
    "schemaVersion":1
}
```
{% endswagger-response %}
{% endswagger %}

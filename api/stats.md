# Stats



{% swagger method="get" path="" baseUrl="https://instl.sh/api/stats" summary="Get installation count of all projects that use instl.sh" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200: OK" description="Installation count of all projects that use instl.sh" %}
```javascript
{
    "installer/some_repo/windows": 1337,
    "owner/another_repo/linux": 420, 
    "owner/another_repo/macos": 1234
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/owner/repo" baseUrl="https://instl.sh/api/stats" summary="Get installation count of specific project" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" required="true" name="owner" %}

{% endswagger-parameter %}

{% swagger-parameter in="path" name="repo" required="true" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Installation count per platform" %}
```javascript
{
    "linux": 0,
    "macos": 1,
    "windows": 2
}
```
{% endswagger-response %}
{% endswagger %}

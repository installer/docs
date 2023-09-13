# Stats



{% swagger method="get" path="" baseUrl="https://instl.sh/api/stats" summary="Installation count of all projects that use instl.sh" %}
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

{% swagger method="get" path="/owner/repo" baseUrl="https://instl.sh/api/stats" summary="Installation count of specific project" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" required="true" name="owner" type="String" %}
Owner of GitHub Repository
{% endswagger-parameter %}

{% swagger-parameter in="path" name="repo" required="true" type="String" %}
GitHub Repository name
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

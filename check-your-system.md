---
description: You can check if Instl runs on your system
---

# Check Your System

## Using The Web Command

{% hint style="info" %}
No need to install anything, just run this command and Instl will check if it can run on your system.
{% endhint %}

{% tabs %}
{% tab title="Linux" %}
```bash
curl -sSL instl.sh/check/linux | bash
```
{% endtab %}

{% tab title="MacOS" %}
```bash
curl -sSL instl.sh/check/macos | bash
```
{% endtab %}

{% tab title="Windows" %}
```powershell
iwr instl.sh/check/windows | iex
```
{% endtab %}
{% endtabs %}

## Using a Local Installation

{% hint style="info" %}
If you have installed Instl locally, you can use the following command.
{% endhint %}

```bash
instl check
```

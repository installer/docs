---
description: Useful for debugging, or if you just like to see what is going on
---

# Verbose Output

## Get Verbose Output

Instl makes it super easy to get verbose output.

Instead of:

<pre class="language-url"><code class="lang-url"><strong>instl.sh/username/reponame/platform
</strong></code></pre>

You can use:

```url
instl.sh/username/reponame/platform/verbose
```

So if you're on Linux, and you want to see verbose output for our `instl-demo` repo, you can use:

```bash
curl -sSL instl.sh/installer/instl-demp/linux/verbose | bash
```

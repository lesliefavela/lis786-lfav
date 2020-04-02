---
title: Menu
layout: default
permalink: /menu/

---
{% for churro in site.churro_cafe %}
{{ churro.title }}
{{ churro.content }}
{{% endfor %}}

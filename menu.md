---
title: Menu
layout: default
permalink: /menu/

---
{% for churros in site.churro_cafe %}
{{ churros.title }}
{{ churros.content }}
{{% endfor %}}

---
title: Menu
layout: default
permalink: /menu/

---
# Menu
{% for churros in site.churro_cafe %}
{{ churros.title }}
{{ churros.content }}
{{% endfor %}}

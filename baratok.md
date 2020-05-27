---
layout: default
title: Barátok lapja
---
# Barátok lapja

{% assign pdfs = site.static_files | where: "type", "pdf" | reverse %}
<ul>
  {% for pdf in pdfs %}
    <li><a href="{{ pdf.path }}">{{ pdf.basename }}</a></li>
  {% endfor %}
</ul>

---
layout: default
title: Barátok lapja

---
# Barátok lapja

A Ferences Plébánia Tájékoztatóját 2018. szeptemberében hívtuk életre. Azóta havonta jelenik meg a kiadvány papír alapon és elektronikusan. A koronavírus miatt kialakult helyzetben nem tudtuk kinyomtatni a 2020 áprilisi és 2020 májusi számot, de kissé bővebb terjedelemben plébániánk honlapján megjelentettük.

Jó olvasást,böngészést kívánunk!

{% assign pdfs = site.static_files | where: "type", "pdf" | reverse %}
<ul>
{% for pdf in pdfs %}
<li><a href="{{ pdf.path }}">{{ pdf.basename }}</a></li>
{% endfor %}
</ul>
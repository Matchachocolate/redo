---
title: Female in Space
layout: index_layout
---

<div class="main-container">
    {% for astronaut_sorted in site.data.info %}
        {% assign astronaut = site.astronauts | find:"name", astronaut_sorted.name %}
    <div class="text-wrapper">
        <div class="ait">
            <h2>{{ astronaut_sorted.year }}</h2>
            <h3><a class="tl" href="{{ astronaut.url }}">{{ astronaut.name }}</a></h3>
            <p>{{ astronaut_sorted.record }}</p>
            <p>{{ astronaut_sorted.time-in-space }} in space</p>
        </div>
    </div>
    {% endfor %}
</div>


---
title: Female in Space
layout: index_layout
---

<div class="main-container">
    {% for astronaut in site.astronauts %}
    <div class="text-wrapper">
        <div class="ait">
            <h2>{{ astronaut.year }}</h2>
            <h3><a href="{{ astronaut.url }}">{{ astronaut.name }}</a></h3>
            <p>{{ astronaut.record }}</p>
            <p>{{ astronaut.time-in-space }}</p>
        </div>
    </div>
    {% endfor %}
</div>


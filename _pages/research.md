---
layout: page
title: Research
shorttitle: research
permalink: /research/
#description: A growing collection of your cool projects.
---

{% for project in site.projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}


We are members of the 
[Hidden Symmettries and Fusion Energy](https://hiddensymmetries.princeton.edu/) collaboration.
Our group's research is funded by grants from the <a href="https://www.energy.gov/science/fes/fusion-energy-sciences">United States Department of Energy</a>, <a href="https://www.pppl.gov/">Princeton Plasma Physics Laboratory</a>,
and
<a href="https://www.simonsfoundation.org/">The Simons Foundation</a>.
---
layout: default
permalink: /about/team
title: 'Our Team'
---

# Our Team

<div class="ui hidden divider"></div>
<div class="ui hidden divider"></div>
<div class="ui four stackable cards">
  {% for thisAuthor in site.data.team limit:5 %}
    <div class="basic card">
      <img src="{{ thisAuthor.pic }}" class="ui centered medium image" alt="Photo of {{ thisAuthor.name }}">
      <div class="content">
        <div class="header">{{ thisAuthor.name }}</div>
        <div class="meta">
          <span class="date">{{ thisAuthor.desig}}</span>
        </div>
        <div class="description">
          {{ thisAuthor.bio }}
        </div>
      </div>
    </div>
  {% endfor %}
</div>
<h2 class="ui header">Advisors</h2>
<div class="ui four stackable cards">
  {% for thisAuthor in site.data.team offset:5 %}
    <div class="basic card">
      <img src="{{ thisAuthor.pic }}" alt="Photo of {{ thisAuthor.name }}">
      <div class="content">
        <div class="header">{{ thisAuthor.name }}</div>
        <div class="meta">
          <span class="date">{{ thisAuthor.desig}}</span>
        </div>
        <div class="description">
          {{ thisAuthor.bio }}
        </div>
      </div>
    </div>
  {% endfor %}
</div>

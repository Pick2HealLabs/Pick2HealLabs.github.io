---
layout: post
permalink: /about/team
title: 'Our Team'
---

<div class="ui hidden divider"></div>
<div class="ui hidden divider"></div>
<div class="ui three column grid">
  {% for thisAuthor in site.data.team limit:3 %}
  <div class="column">
    <div class="ui fluid raised card">
      <div class="blurring dimmable image">
        <div class="ui dimmer">
          <div class="content">
            <div class="center">
              <div>{{ thisAuthor.bio }}</div>
            </div>
          </div>
        </div>
        <img src="{{ thisAuthor.pic }}" alt="Photo of {{ thisAuthor.name }}">
      </div>
      <div class="content">
        <div class="header">{{ thisAuthor.name }}</div>
        <div class="meta">
          <span class="date">{{ thisAuthor.desig}}</span>
        </div>
      </div>
    </div>
    </div>
{% endfor %}
</div>

<div class="ui three column grid">
  {% for thisAuthor in site.data.team offset:4 limit:1 %}
  <div class="column">
    <div class="ui fluid card">
      <div class="blurring dimmable image">
        <div class="ui dimmer">
          <div class="content">
            <div class="center">
              <div>{{ thisAuthor.bio }}</div>
            </div>
          </div>
        </div>
        <img src="{{ thisAuthor.pic }}" alt="Photo of {{ thisAuthor.name }}">
      </div>
      <div class="content">
        <div class="header">{{ thisAuthor.name }}</div>
        <div class="meta">
          <span class="date">{{ thisAuthor.desig}}</span>
        </div>
      </div>
    </div>
    </div>
{% endfor %}
</div>

<h1 class="ui massive header">Advisors</h1>
<div class="ui three column grid">
  {% for thisAuthor in site.data.team offset:5 %}
  <div class="column">
    <div class="ui fluid card">
      <div class="blurring dimmable image">
        <div class="ui dimmer">
          <div class="content">
            <div class="center">
              <div>{{ thisAuthor.bio }}</div>
            </div>
          </div>
        </div>
        <img src="{{ thisAuthor.pic }}" alt="Photo of {{ thisAuthor.name }}">
      </div>
      <div class="content">
        <div class="header">{{ thisAuthor.name }}</div>
        <div class="meta">
          <span class="date">{{ thisAuthor.desig}}</span>
        </div>
      </div>
    </div>
    </div>
{% endfor %}
</div>

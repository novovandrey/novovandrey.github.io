---
layout: default
title: "Engineering Notes"
description: "Practical engineering notes on Java, JVM, system design, distributed systems and interview preparation."
permalink: /engineering-notes/
---

<section class="hero">
  <p class="eyebrow">Technical writing</p>
  <h1>Engineering Notes</h1>
  <p class="hero-text">
    Practical notes on Java, JVM, system design, distributed systems, databases,
    and software engineering interviews.
  </p>
</section>

<section class="notes-list">
  {% if site.posts.size > 0 %}
    {% for post in site.posts %}
      <article class="note-card">
        <div class="note-meta">
          <time datetime="{{ post.date | date_to_xmlschema }}">
            {{ post.date | date: "%B %d, %Y" }}
          </time>

          {% if post.tags %}
            <span>·</span>
            <span>{{ post.tags | join: ", " }}</span>
          {% endif %}
        </div>

        <h2>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h2>

        {% if post.description %}
          <p>{{ post.description }}</p>
        {% endif %}
      </article>
    {% endfor %}
  {% else %}
    <p>No articles yet.</p>
  {% endif %}
</section>

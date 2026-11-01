---
layout: page
title: Events
subtitle: Conferences, schools, talks, and posters.
slug: events
permalink: /events/
---

{% assign schools = site.data.events | where: "type", "School" %}
{% assign conferences = site.data.events | where: "type", "Conference" %}
{% assign talks = site.data.events | where: "type", "Talk" %}
{% assign posters = site.data.events | where: "type", "Poster" %}

{% include event-group.html heading="Talks" items=talks %}
{% include event-group.html heading="Posters" items=posters %}
{% include event-group.html heading="Schools" items=schools %}
{% include event-group.html heading="Conferences Attended" items=conferences %}

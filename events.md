---
layout: page
title: Events
subtitle: Conferences, summer schools, talks, and posters.
slug: events
permalink: /events/
---

{% assign summer_schools = site.data.events | where: "type", "Summer School" %}
{% assign conferences = site.data.events | where: "type", "Conference" %}
{% assign talks = site.data.events | where: "type", "Talk" %}
{% assign posters = site.data.events | where: "type", "Poster" %}

{% include event-group.html heading="Talks" items=talks %}
{% include event-group.html heading="Posters" items=posters %}
{% include event-group.html heading="Summer Schools" items=summer_schools %}
{% include event-group.html heading="Conferences Attended" items=conferences %}

---
layout: page
title: Seminar
permalink: /seminar/
nav: true
nav_order: 3
---

The CRaFT Lab Seminar Series brings together researchers working across the areas of 
Formal Methods, Automated Reasoning, Artificial Intelligence, and theoretical Mathematics. 
Talks are held monthly on Thursdays at 3:00 PM CT and are open to all.

To receive announcements, join our mailing list:

<!-- Mailchimp signup embed goes here once configured -->
<div style="margin: 1.5rem 0; padding: 1rem; 
            background: #f8f9fa; border-radius: 8px;">
  <strong>Get Email Reminders:</strong> Mailing list signup coming soon. 
  In the meantime, contact 
  <a href="mailto:jstubbs@tacc.utexas.edu">jstubbs@tacc.utexas.edu</a> 
  to be added to the seminar announcements list.
</div>

---

## Upcoming Talks

{% assign upcoming = site.seminars | where: "upcoming", true | sort: "date" %}
{% if upcoming.size > 0 %}
  {% for seminar in upcoming %}
<div style="margin-bottom: 2rem; padding: 1.25rem; 
            border-left: 4px solid #4a90d9; background: #f8f9fa; 
            border-radius: 0 8px 8px 0;">
  <p style="margin: 0 0 0.25rem 0;">
    <strong>{{ seminar.date | date: "%B %-d, %Y" }}</strong> 
    &nbsp;·&nbsp; {{ seminar.time }} 
    &nbsp;·&nbsp; {{ seminar.location }}
  </p>
  <h3 style="margin: 0.5rem 0;">{{ seminar.title }}</h3>
  <p style="margin: 0 0 0.5rem 0;">
    <strong>{{ seminar.speaker }}</strong>, {{ seminar.affiliation }}
  </p>
  {% if seminar.abstract %}
  <details>
    <summary style="cursor: pointer; color: #4a90d9;">Abstract</summary>
    <p style="margin-top: 0.75rem;">{{ seminar.abstract }}</p>
  </details>
  {% endif %}
  {% if seminar.website %}
  <p style="margin-top: 0.5rem; margin-bottom: 0;">
    <a href="{{ seminar.website }}" target="_blank">Speaker website</a>
  </p>
  {% endif %}
</div>
  {% endfor %}
{% else %}
<p><em>No upcoming talks currently scheduled. Check back soon!</em></p>
{% endif %}

---

## Past Talks

{% assign past = site.seminars | where: "upcoming", false | sort: "date" | reverse %}
{% if past.size > 0 %}
  {% for seminar in past %}
<div style="margin-bottom: 1.5rem; padding: 1rem; 
            border-left: 4px solid #adb5bd; background: #f8f9fa;
            border-radius: 0 8px 8px 0;">
  <p style="margin: 0 0 0.25rem 0;">
    <strong>{{ seminar.date | date: "%B %-d, %Y" }}</strong>
    &nbsp;·&nbsp; {{ seminar.time }}
  </p>
  <h3 style="margin: 0.5rem 0;">{{ seminar.title }}</h3>
  <p style="margin: 0 0 0.5rem 0;">
    <strong>{{ seminar.speaker }}</strong>, {{ seminar.affiliation }}
  </p>
  {% if seminar.abstract %}
  <details>
    <summary style="cursor: pointer; color: #6c757d;">Abstract</summary>
    <p style="margin-top: 0.75rem;">{{ seminar.abstract }}</p>
  </details>
  {% endif %}
  <p style="margin-top: 0.5rem; margin-bottom: 0;">
    {% if seminar.slides != "" %}
    <a href="{{ seminar.slides }}" target="_blank">Slides</a> &nbsp;·&nbsp;
    {% endif %}
    {% if seminar.recording != "" %}
    <a href="{{ seminar.recording }}" target="_blank">Recording</a>
    {% endif %}
  </p>
</div>
  {% endfor %}
{% else %}
<p><em>No past talks yet — our seminar series is just getting started!</em></p>
{% endif %}
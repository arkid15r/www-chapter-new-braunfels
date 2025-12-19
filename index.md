---

layout: col-sidebar
title: OWASP New Braunfels
tags: chapter, New Braunfels, Texas, NBTX
region: North America
meetup-group: owasp-new-braunfels-chapter

---

<!-- rebuild 001 -->

{% include top_nav.md page="home" %}

<br/><br/>

## Welcome
Started in 2022, the OWASP New Braunfels chapter is located in a small town in the Central Texas Hill Country. Surrounded by San Marcos and Austin to the north and San Antonio to the south, [New Braunfels](https://nbtexas.org/) is home to many technology workers. This chapter
exists to bring application security awareness to New Braunfels and the surrounding communities. 

## Participation
The Open Worldwide Application Security Project (OWASP) is a nonprofit foundation that works to improve the security of software. All our members and participants are encouraged to become an [OWASP Member](https://owasp.org/membership/)

If you are interested in participating in the OWASP New Braunfels Chapter please feel free to join us at our next meeting, listed below. We are always looking for people who would like to present at one of our meetings; if that sounds like something you would
be interested in, please drop an email to one of the leaders (listed to the right).


Upcoming Activities
---------------------
{% if site.data.activities.size > 0 %}
{% assign activities = site.data.activities | sort: "start-date" %}
{% for activity in activities %}
<hr>
{:class='activity'}
* ### {{ activity.name }}

  **What: {{ activity.type | capitalize }}**<br>
  **Date: {{ activity.start-date }}{% if activity.start-date != activity.end-date %} - {{ activity.end-date }}{% endif %}**<br>
  **Time: {{ activity.start_time }} - {{ activity.end_time }}**<br>
  **Where: {{ activity.where }}**<br>
  **[RSVP]({{ activity.rsvp_url }})**<br>
  **Description:**
  {{ activity.description }}<br>

{% endfor %}
{% else %}
None currently scheduled
{% endif %}

---
layout: page
title: Home
nav_order: 1
description: A week-to-week description of the content covered in the course.
---

# Data 102: Data, Inference, and Decisions

{: .mb-2 }
UC Berkeley, Spring 2024
{: .mb-0 .fs-6 .text-grey-dk-000 }

<div>
{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
  <div class="role">
    {% for staffer in instructors %}
    {{ staffer }}
    {% endfor %}
  </div>
</div>

{% assign announcement = site.announcements | where: 'week', site.current_week %}
{{ announcement }}


## Schedule
[**Jump to current week**](#week-{{ site.current_week }}){: .btn }

{: .warning }
The calendar is currently under construction, and is subject to change until this warning has been removed.

{% for module in site.modules %}
{{ module }}
{% endfor %}
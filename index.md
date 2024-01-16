---
layout: page
title: Home
nav_order: 1
description: A week-to-week description of the content covered in the course.
course:
  edstem: 
  faq: 
current_week: week-1-binary-decisions
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

{% assign announcement = site.announcements | last %}
{{ announcement }}


<a name="schedule"></a>
## Schedule
[**Jump to current week**](#{{page.current_week}}){: .btn }
{: .warning }
The calendar is currently under construction, and is subject to change until this warning has been removed.

{% for module in site.modules %}
{{ module }}
{% endfor %}
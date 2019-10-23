---
layout: page
title: Students
permalink: /students/
---


<ul class="students">
{% for student in site.data.students %}
  <li class="student">
    <img class="student--image" src="https://i.pravatar.cc/150?img={{forloop.index}}">
    <div class="student--info">
      <p class="student--name">{{student.firstname}} {{student.lastname}}</p>
      <p class="student--project">{{student.project}}</p>
      <a href="mailto:{{student.email}}">
        {{ student.email }}
      </a>
    </div>
  </li>
{% endfor %}
</ul>
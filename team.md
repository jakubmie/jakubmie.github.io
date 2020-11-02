---
title: Team
permalink: /team/
---

{% assign team_sorted = site.team | sort: 'sort_name' %}

### Team

<div class="content list team">
  {% for profile in team_sorted %}
      {% if profile.position == 'alumnus' or profile.position == 'disable' %}
        {% continue %}
      {% endif %}
      <div class="list-item-team">
        <p class="list-post-title">
          {% if profile.avatar %}
           <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="{{site.baseurl}}/images/team/{{profile.avatar}}"></a>
          {% else %}
           <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="http://evansheline.com/wp-content/uploads/2011/02/.jpg"></a>
          {% endif %}
          <a class="profname">{{ profile.name }}</a><br><a class="name" href="mailto:{{ profile.email }}">{{ profile.email }}</a>
        </p>
      </div>    
  {% endfor %}
</div>

<hr>

[Code of Conduct](/assets/docs/lab_code_of_conduct)

<hr>

### Alumni

* Joanna Tomczak 2020 (master studnet) 

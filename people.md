---
title: People
permalink: /people/
---

{% assign people_sorted = site.people | sort: 'name' %}




<div class="content list people">
  {% for profile in people_sorted %}
      <div class="list-item-people">
        <p class="list-post-title">
          {% if profile.avatar %}
           <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="{{site.baseurl}}/images/people/{{profile.avatar}}"></a>
          {% else %}
           <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="http://evansheline.com/wp-content/uploads/2011/02/.jpg"></a>
          {% endif %}
          <a class="profname">{{ profile.name }}</a><br><a class="name" href="mailto:{{ profile.email }}">{{ profile.email }}</a>
        </p>
      </div>    
  {% endfor %}
</div>




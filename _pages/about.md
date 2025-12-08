---
permalink: /
title: #"Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
classes: about-page
redirect_from: 
  - /about/
  - /about.html
---



I am a Ph.D. Candidate in Robotics and AI, advised by Dr. Julie A. Adams at Oregon State University. 

I graduated with a Masters in Robotics from University of Michigan in May 2021. At UM, I worked at the Laboratory for Progress directed by Dr. Chad Jenkins, and at the UM Ford Center for Autonomous Vehicles. I completed my Bachelors in Electronics and Communication Engineering from VNIT Nagpur, India in May 2018.

My primary research interests are Multiple Robot Systems, Distributed AI, Game Theory, Planning under Uncertainty.



## Recent News

{% assign recent = site.posts | sort: "date" | reverse %}
<ul class="recent-news-list">
  {% for post in recent limit:5 %}
    {% if post.published != false %}
    <li>
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d, %Y" }}</time>
      — {{ post.title }}
    </li>
    {% endif %}
  {% endfor %}
</ul>

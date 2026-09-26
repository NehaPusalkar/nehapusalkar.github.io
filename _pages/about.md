---
permalink: /
title: #"Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
classes: about-page
redirect_from: 
  - /about/
  - /about.html
---



I am a Ph.D. Candidate in Robotics and AI, advised by [Dr. Julie A. Adams](https://engineering.oregonstate.edu/people/julie-adams) at Oregon State University. My dissertation develops scalable coaltition formation algoritms for heterogeneous multi-robot collectives of up to 10,000 robots. I utilize game-theoretic and sequential decision-making techniques to design distributed coordination frameworks for dynamic and uncertain environments. I envision developing hybrid AI systems integrating foundation model reasoning with game-theoretic coordination guarantees for long-duration autonomy.

I graduated with a Masters in Robotics from the University of Michigan, Ann Arbor in May 2021. At UM, I worked at the Laboratory for Progress directed by [Dr. Chad Jenkins](https://robotics.umich.edu/people/faculty/chad-jenkins/), and at the UM Ford Center for Autonomous Vehicles. I completed my Bachelors in Electronics and Communication Engineering from VNIT Nagpur, India in May 2018.

<u>Research Interests</u>:

* Multi-Robot Systems and Large Scale Collectives: Task Allocation and Planning
* Multi-Objective Optimization
* Game Theory
* Reinforcement Learning

<div class="home-callout">
  <p class="home-callout__lead">I am open to industry/academic research positions starting January 2027.</p>
  <p class="home-callout__sub">Feel free to reach out if I might be a good fit for your organization.</p>
</div>

## Recent News

{% assign recent = site.posts | sort: "date" | reverse %}
<ul class="recent-news-list">
  {% for post in recent limit:7 %}
    {% if post.published != false %}
    <li>
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %Y" }}</time>: {{ post.title }}
    </li>
    {% endif %}
  {% endfor %}
</ul>

---
layout: default
title: Home
---

## Welcome to the Behavioural Economics Laboratory at UWA!      


<p> The Behavioural Economics Laboratory (BEL) was created in 2013-2014 jointly by the <a href="http://www.csiro.au">Commonwealth Scientific and Industrial Research Organisation (CSIRO)</a>, the <a href="http://www.psychology.uwa.edu.au">UWA School of Psychology</a> and the <a href="http://www.are.uwa.edu.au">UWA School of Agricultural and Resource Economics</a>, both in the Faculty of Science. Its focus echoes the joint 2002 Nobel Prize that brought together the two disciplines of psychology and economics into what is now referred to as Behavioural Economics. </p>

<p> The BEL at UWA is a computer lab of just under 20 machines that are interconnected to allow real-time interactions between lab participants, either individually or as groups. The main purpose of the three founding entities was to study human behaviour with respect to the natural environment. Issues such as contribution to public environmental goods, participation in environmental auctions, the willingness to co-operate to achieve super-additive environmental outcomes, the role of perceived fairness, risk prevention and willingness to pay for it, and the factors influencing the effectiveness of information or education campaigns on environmental behaviour are some of the areas on the current research agenda. </p>

<p> A number of Masters and PhD students have begun or will start using the lab to carry out experiments investigating some of the above issues, and current as well as new research projects are under way. </p>

<div class="posts">
  {% for post in paginator.posts %}
  <div class="post">
    <h1 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>

    <span class="post-date">{{ post.date | date_to_string }}</span>

    {{ post.content }}
  </div>
  {% endfor %}
</div>

<div class="pagination">
  {% if paginator.next_page %}
    <a class="pagination-item older" href="{{ site.baseurl }}page{{paginator.next_page}}">Older</a>
  {% else %}
    <span class="pagination-item older">Older</span>
  {% endif %}
  {% if paginator.previous_page %}
    {% if paginator.page == 2 %}
      <a class="pagination-item newer" href="{{ site.baseurl }}">Newer</a>
    {% else %}
      <a class="pagination-item newer" href="{{ site.baseurl }}page{{paginator.previous_page}}">Newer</a>
    {% endif %}
  {% else %}
    <span class="pagination-item newer">Newer</span>
  {% endif %}
</div>
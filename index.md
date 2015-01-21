---
layout: default
title: Home
---

## Welcome to the Behavioural Economics Laboratory at UWA!      

<p> The Behavioural Economics Laboratory (BEL) was created in 2013-2014 jointly by the Commonwealth Scientific and Industrial Research Organisation (CSIRO), the UWA School of Psychology and the UWA School of Agricultural and Resource Economics, both in the Faculty of Science. Its focus echoes the joint 2002 Nobel Prize that brought together the two disciplines of psychology and economics into what is now referred to as Behavioural Economics. 

The BEL at UWA is a computer lab of just under 20 machines that are interconnected to allow real-time interactions between lab participants, either individually or as groups. The main purpose of the three founding entities was to study human behaviour with respect to the natural environment. Issues such as contribution to public environmental goods, participation in environmental auctions, the willingness to co-operate to achieve super-additive environmental outcomes, the role of perceived fairness, risk prevention and willingness to pay for it, and the factors influencing the effectiveness of information or education campaigns on environmental behaviour are some of the areas on the current research agenda. </p>

<!--## Research interests

*Auditory distraction:* testing a duplex mechanism account of auditory distraction and attentional selectivity in which some forms of distraction are resistible and others are ineluctable.

*Behavioural economics:* applying insights from laboratory experiments and psychology to economics, particularly the economics of climate change and other ecosystem issues.

*Cognitive modelling:* computational and mathematical modelling of cognitive processes; model evaluation and selection issues; models of choice behaviour and response time.

*Human memory:* short-term and long-term memory; serial recall memory; free recall memory; sequence learning; relationship between time and memory.

*Psychology and climate change:* using principles of cognitive and social psychology to facilitate the communication of climate science.

<br/> -->

<!--
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
---
layout: default
---

<br><br>
<div class="posts">
  {% for post in site.posts %}
    {% case post.layout %}
    {% when "status" %}
      <div class="status">
        <h1 class="status-content">{{post.content}}</h1>
        <div class='post-footer'>
          <div class='left'><div class='share-link' data-link="{{post.url}}"></div></div>
          <a href="{{ post.url }}"><span class="post-date">{{ post.date | date_to_string }}</span></a>
        </div>
      </div>
    {% when "image" %}
      <div class="slide">
        <img src="{{post.source}}" title="{{post.title}}">
        {{post.content}}
        <div class='post-footer'>
          <div class='left'><div class='share-link' data-link="{{post.url}}"></div></div>
          <a href="{{ post.url }}"><span class="post-date">{{ post.date | date_to_string }}</span></a>
        </div>
      </div>
    {% else %}
      <div class="post">
        <h1 class="post-title">
          <a href="{{ post.url }}">
            {{ post.title }}
          </a>
        </h1>

        <span class="post-date">{{ post.date | date_to_string }}</span>

        {{ post.content }}
        <div class='post-footer'>
          <div class='share-link' data-link="{{post.url}}"></div>
        </div>
      </div>
    {% endcase %}
      <br>
      <br>
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

<!-- <div class="posts">
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
</div> -->
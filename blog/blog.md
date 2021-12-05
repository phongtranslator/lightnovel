---
title: projects
layout: page
permalink: "/blog/"
description: null
nav: true
display_categories:
- Nguyệt đạo dị giới
- Tensei shitara Slime Datta Ken
horizontal: false  
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 10
  sort_field: date
  sort_reverse: true
  trail:
    before: 1 # The number of links before the current page
    after: 3  # The number of links after the current page

---

<div class="projects">
  {% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
    {% for category in page.display_categories %}
      <h2 class="category">{{ category}}</h2>
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
      <div class="table-responsive">        
        <table class="table table-sm table-borderless">
          {% for post in paginator.posts %}
          {% assign cata = category |  replace:" ", "-" %}
          {% assign postcata = post.categories |  join:"" %}
          {% if postcata == cata %}
          <tr>            
            <a class="news-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>            
          </tr>
          {%endif%}
          {% endfor %}
        </table>
      </div>

  {% include pagination.html %}
    {% endfor %}
  {% endif %}

</div>

{% for post in paginator.posts %}
  <article class="blog-post">
    <div>
      <h2>
        <a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}
      </a>
      </h2>
      <div class="entry">
        {{ post.excerpt }}
      </div>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </div>
  </article>
{% endfor %}

{% if paginator.total_pages > 1 %}
  <div class="Pagination">
    {% if paginator.previous_page %}
      <a class="link-highlight" href="{{ paginator.previous_page_path | prepend: site.baseurl }}">Newer</a>
    {% endif %}
    {% if paginator.next_page %}
      <a class="link-highlight" href="{{ paginator.next_page_path | prepend: site.baseurl }}">Older</a>
    {% endif %}
  </div>
{% endif %}

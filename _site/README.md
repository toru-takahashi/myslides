<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      <ul>
        <li>Event Name: {{post.event}}</li>
        <li>Event Date: <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time></li>
      </ul>
    </li>
  {% endfor %}
</ul>
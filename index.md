[about me](/about) | [schedule](/schedule)

## Knowledge system

- [what is computer](/computer)
- [algorithm](/algorithm-learning)
- [cpp learning](/cpp-learning)
- [operating system](/operating-system)
- [web-based programming](/web-program)
- [english](/english) 
- [geometry](/geometry)
- [advanced algebra](/algebra)
- [theory of numbers](/theory-of-numbers)

## Random notes

{% assign posts_by_year = site.posts | group_by_exp:"post", "post.date | date: '%Y' " %}
{% for group in posts_by_year %}

<h3>{{ group.name }}</h3>
<ul>
    {% for post in group.items %}
    <li><div style="width:60px;float:left;">{{ post.date | date: "%b %-d" }}</div> <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}
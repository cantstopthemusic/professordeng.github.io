[about](/about) | [schedue](/schedule)

- [crazy laboratory](/lab)

## computer science

- [what is computer](/computer)
- [algorithm](/algorithm-learning)
- [c learning](/c-learning)
- [c++ learning](/cpp-learning)
- [operating system](/operating-system)
- [web program](/web-program)
- [english](/english) 
- [python learning](/python-learning)
- [artificial intelligence](/ai)
- [computer network](/computer-network)
- [embedded design](/embedded-design)
- [programing language](/programming-language)

## mathematics

- [theory of numbers](/theory-of-numbers)
- [geometry](/geometry)
- [algebra](/algebra)

## notes

{% assign posts_by_year = site.posts | group_by_exp:"post", "post.date | date: '%Y' " %}
{% for group in posts_by_year %}

<h3>{{ group.name }}</h3>
<ul>
    {% for post in group.items %}
    <li><div style="width:60px;float:left;">{{ post.date | date: "%b %-d" }}</div> <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}
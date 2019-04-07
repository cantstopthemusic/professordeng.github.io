[关于](/about) | [日程](/mytime)

## 计算机

- [what is computer](/computer)
- [algorithm](/algorithm)
- [cpp learning](/cpp-learning)
- [operating system](/operating-system)
- [web-based programming](/web-program)

## 语言

- [english](/english)

## 生活

- [life](/life)
- [exercise](/exercise)

## 数学

- [geometry](/geometry)
- [advanced algebra](/algebra)
- [theory of numbers](/theory-of-numbers)

## 散记 

{% assign posts_by_year = site.posts | group_by_exp:"post", "post.date | date: '%Y' " %}
{% for group in posts_by_year %}

<h3>{{ group.name }}</h3>
<ul>
    {% for post in group.items %}
    <li><div style="width:60px;float:left;">{{ post.date | date: "%b %-d" }}</div> <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}
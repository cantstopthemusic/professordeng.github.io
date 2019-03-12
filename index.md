简单点，写作的方式简单点。[关于我](/about)

## 计算机

- [computer](/computer)
- [cpp learning](/cpp-learning)
- [computer system](/OS)

## 语言

- [english](/english)

## 生活

- [life](/life)
- [exercise](/exercise)

## 数学

- [geometry](/geometry)
- [advanced algebra](/algebra)

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
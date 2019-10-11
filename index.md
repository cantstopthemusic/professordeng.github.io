[about me](/about) | [resources](/resources)

## computer science

- [algorithm](/algorithm-learning)
- [artificial intelligence](/ai)
- [c learning](/c-learning)
- [c++ learning](/cpp-learning)
- [computer security](/computer-security)
- [computer network](/computer-network)
- [computer world](/computer)
- [data structure](/data-structure)
- [embedded design](/embedded-design)
- [linux learning](/linux-learning)
- [opengl learning](/opengl-learning)
- [operating system](/operating-system)
- [python learning](/python-learning)
- [programing language](/programming-language)
- [principle of computer composition](/computer-system)
- [web program](/web-program)

## mathematics

- [advanced mathematics](/advanced-mathematics)
- [algebra](/algebra)
- [geometry](/geometry)
- [graph theory](/graph-theory)
- [numerical analysis](/numerical-analysis)
- [probability theory](/probability-theory)
- [theory of numbers](/theory-of-numbers)

## language

- [english](/english)

## other

- [crazy laboratory](/lab)
- [learning theory](/learning-theory)
- [philosophy](/philosophy)
- [politics](/politics)
- [willpower training](/self-control)

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
[关于](/about) | [行程](/schedule)

- [疯狂实验室](/lab)

## 计算机科学

- [计算机科学](/computer)
- [算法](/algorithm-learning)
- [c 学习笔记](/c-learning)
- [c++ 学习笔记](/cpp-learning)
- [操作系统](/operating-system)
- [web 编程](/web-program)
- [英语](/english) 
- [python 学习笔记](/python-learning)
- [人工智能](/ai)
- [计算机网络](/computer-network)
- [嵌入式设计](/embedded-design)
- [编程语言](/programming-language)

## 数学

- [数论](/theory-of-numbers)
- [几何](/geometry)
- [高等代数](/algebra)

## 随笔

{% assign posts_by_year = site.posts | group_by_exp:"post", "post.date | date: '%Y' " %}
{% for group in posts_by_year %}

<h3>{{ group.name }}</h3>
<ul>
    {% for post in group.items %}
    <li><div style="width:60px;float:left;">{{ post.date | date: "%b %-d" }}</div> <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}
[Truth](/truth) | [Resources](/resources)

## Computer Science

- [Algorithm](/algorithm-learning)
- [Artificial Intelligence](/ai)
- [C](/c-learning)
- [C++ ](/cpp-learning)
- [Computer Security](/computer-security)
- [Computer Network](/computer-network)
- [Computer World](/computer)
- [Data structure](/data-structure)
- [Embedded Design](/embedded-design)
- [Linux](/linux-learning)
- [OpenGL](/opengl-learning)
- [Operating System](/operating-system)
- [Python](/python-learning)
- [Programming Language](/programming-language)
- [Principle of Computer Composition](/computer-system)
- [XV6](/xv6-book)
- [WEB](/web-program)

## Mathematics

- [Advanced Mathematics](/advanced-mathematics)
- [Algebra](/algebra)
- [Geometry](/geometry)
- [Graph Theory](/graph-theory)
- [Numerical Analysis](/numerical-analysis)
- [Probability Theory](/probability-theory)
- [Theory of Numbers](/theory-of-numbers)

## Language

- [English](/english)

## Other

- [Crazy Lab](/lab)
- [Learning Theory](/learning-theory)
- [Philosophy](/philosophy)
- [Politics](/politics)
- [Psychoanalysis](/psychoanalysis)
- [Willpower](/self-control)

## Notes

{% assign posts_by_year = site.posts | group_by_exp:"post", "post.date | date: '%Y' " %}
{% for group in posts_by_year %}

<h3>{{ group.name }}</h3>
<ul>
    {% for post in group.items %}
    <li><div style="width:60px;float:left;">{{ post.date | date: "%b %-d" }}</div> <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}


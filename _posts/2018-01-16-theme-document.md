---
title: How to build a blog
---

[Jekyll](https://jekyllrb.com) is a simple, extendable, static site generator officially supported by GITHUB. You give it text written in your favorite markup language and it churns through layouts to create a static website. 

## Building Process

- [a github account](https://github.com)

  If you don't know what is GITHUB, just google. 

- [github desktop](https://git-scm.com/)

  Use it to transfer files between local and server.

- [ruby](https://rubyinstaller.org/downloads/)

  JEKYLL is based on ruby.

- [domain](https://cloud.tencent.com/) (optional)

  GITHUB will provide a domain name called `usename.github.io` to you. also you can bind personal domain name for you website.

- [Jekyll Docs](https://jekyllrb.com/)

- [Jekyll themes](https://jekyllthemes.org/)

## Typography

### Picture
![图标](/img/example.jpg)

### Quote
> I think, therefore I am -- René Descartes

### Code
``` c++
#include <iostream>

using namespace std;

int main(){
    cout << "Hello World!";
    return 0;
}
```

### Font style

- **bold**
- *italics*
- `highlight`
- ~~delete~~
- <u>underline</u>

### Table

| name  | ID   | score |
| ----- | ---- | ----- |
| David | 1    | 98    |
| Nancy | 2    | 99    |
| Curry | 3    | 101   |

## Formula

if you need formula rendering, add `site.math` to the end of page.


$$
\frac{\mathrm{d}}{\mathrm{d}t} \left ( \frac {\partial L}{\partial \dot{q}_j} \right ) = \frac {\partial L}{\partial q_j}
$$

### Video

<video src="https://cdn-video.xinpianchang.com/5b7fc02a84108.mp4" width = "100%" controls="" preload=""></video>
{{site.math}}
---
layout: archive
title: "Publication"
permalink: /publication/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

[1] T. Hu, Y. Deng, Y. Deng and A. Ge, "Fully Convolutional Network Variations and Method on Small Dataset," 2021 IEEE
International Conference on Consumer Electronics and Computer Engineering (ICCECE), 2021, pp. 40-46, doi:
10.1109/ICCECE51280.2021.9342059. [download.pdf](https://github.com/TianyouHu/tianyouhu.github.io/files/10928792/download.pdf)



---
layout: homepage.liquid
title: Matthew Collins
---

Hello World

## About

* Founder of NoeticOS
* Chief Product Officer at Rosemark
* Former CS Teacher, Head of Entrepreneurship, Rowing Coach at Eton College

## Blog

<ul>
{% if collections.blog.size > 0 %}
{% for post in collections.blog reversed %}
    {% if post.data.draft != true %}
    <li><a href="{{ post.url }}">{{ post.data.title }} - {{ post.date | date: "%d-%m-%Y" }}</a></li>
    {% else %}
    <li>{{ post.data.title }} - {{ post.date | date: "%d-%m-%Y" }} (draft)</li>
    {% endif %}
{% endfor %}
{% else %}
    <li>No posts found</li>
{% endif %}
</ul>


## Contact

* [LinkedIn](https://www.linkedin.com/in/i-matthewcollins/)
* [Twitter](https://twitter.com/imatthewcollins)
* [GitHub](https://github.com/itsmcollins)

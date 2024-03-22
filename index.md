---
layout: page
---

### Hi there!
I’m Alvise Memo, I was born near Venice, in Italy.
I’ve grown up with passion for mechanics and engineering.
While I was young I experimented on motorcycles to build 
something new and different and that lead me to informatics.
I am mostly intrested in machine learning, music and food.


I graduated in 2013 at the University of Padua in Information Engineering
with a thesis on “Data acquisition with cameras and ToF sensors”.
In 2015 I obtained also a Master degree in Informatics Engineering,
with a work called “Multi-model Head Mounted Vision System with Gesture Interface”.
Currently I work and live in the bay area in California (USA). If you come by
let me know!


### Going deeper:
* [Publications](https://scholar.google.com/citations?user=gTVBw7UAAAAJ)
* [LinkedIn](https://www.linkedin.com/in/alvise-m/)
* [Github](https://github.com/alvisememo)

### My posts:
This is a collection of posts written for reference or to help anyone intrested:

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

---
permalink: /reading/
title: "Reading"
author_profile: true
redirect_from: 
  - /readings/
  - /readings.html
---


I am a huge fan of writers Helene Wecker, Patrick Radden Keefe, and Ted Chiang. I am a religious podcast listener and am particularly fond of The Economist, The Big Story, and Binchtopia. For TV shows, I absolutely love Succession, Derry Girls, and Fleabag. 

<!-- IMPORTANT: to edit the list of books, please go to the folder _data/books.yml and edit according to the format -->
<!-- IMPORTANT: to edit the list of books, please go to the folder _data/books.yml and edit according to the format -->
<!-- IMPORTANT: to edit the list of books, please go to the folder _data/books.yml and edit according to the format -->

{% for entry in site.data.books %}
  <h2>{{ entry.year }}</h2>
  <ol>
    {% for book in entry.books %}
      <li>
        <b>{{ book.title }}</b>, <i>{{ book.author }}</i>
        <p>{{ book.description }} </p>
      </li>
    {% endfor %}
  </ol>
{% endfor %}
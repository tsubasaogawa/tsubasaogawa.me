# articles

{% assign doclist = site.pages | sort: 'url' | reverse %}
  {% for doc in doclist %}
    {% if doc.url contains 'articles/' and doc.url != page.url %}

-     [{{ doc.name }}]({{ site.baseurl }}{{ doc.url }})
    {% endif %}
  {% endfor %}

[Back to home](../)

---
layout: none
title: Contents
---
# articles

{% assign doclist = site.pages | sort: 'url', 'last'  %}
  {% for doc in doclist %}
    {& if doc.url contains 'articles/' and doc.url contains '.md' &}
-     [{{ doc.name }}]({{ site.baseurl }}{{ doc.url }})
	{& endif &}
  {% endfor %}

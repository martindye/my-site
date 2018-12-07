---
permalink: index.html
title: blog.codemartin.com
show_description: true
---

## Welcome

<h5>
If we like an item, we're truthful about it and we're pleased to share our opinion.
We are very fussy, so if an item gets a high opinion, you can bet it's an excellent product.
Admittedly, everyone has different tastes, but if we like something then we're quite sure you will too.
We are enthusiasts who like to write and share opinions with others and we hope you like our unique ways 
of describing things and that you can rely on this blog as a trusted source. We only review things we like
(or love) and you won't find anyting we don't like on this site.

We hope you enjoy the reviews!<br />

Note: <em>As an Amazon Associate I earn from qualifying purchases.</em>
</h5>

{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

<div id="sfcm1kxuwmcfep3fjqwa52ppshsf47hhrxm"></div>
<script type="text/javascript" src="https://counter5.wheredoyoucomefrom.ovh/private/counter.js?c=m1kxuwmcfep3fjqwa52ppshsf47hhrxm&down=async" async></script>
<br><noscript><a href="https://www.freecounterstat.com" title="website counters"><img src="https://counter5.wheredoyoucomefrom.ovh/private/freecounterstat.php?c=m1kxuwmcfep3fjqwa52ppshsf47hhrxm" border="0" title="website counters" alt="website counters"></a></noscript>

---
layout: page
title: About
permalink: /about
comments: false
---

<div class="row justify-content-center">
<div class="col-md-8 pr-5">

<p>This website was created as a collection of resources to help teach CAD and Design for FRC using Onshape (although many concepts could apply to other software) on team <a href="http://littletonrobotics.org/">6328</a>. We decided to open source the resources to help other teams and encourage others to add to and improve the content.</p>

<h4>Meet the Team</h4>

{% for authors in site.data.authors %}
{% assign author = authors[1] %}
{% if author.show == true %}
{% include author.html %}
{% endif %}
{% endfor %}

<h4>Want to see yourself on the list?</h4>

<p>Head over to our <a href="/contribute">contribute page</a> to learn how to help us fix or add more content. We're always looking for feedback.</p>

</div>

</div>

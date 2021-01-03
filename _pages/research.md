---
title: "KuzminLab - Research"
layout: textlay
excerpt: "KuzminLab - Research"
sitemap: false
permalink: /research/
---

# Research


{% assign number_printed = 0 %}
{% for proj in site.data.projlist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if proj.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit class="text-center">{{ proj.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/{{ proj.image }}" class="img-responsive" width="100%" style="float: center" />
  <p>{{ proj.description }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

<!-- Default Statcounter code for Kuzmin Lab
https://kuzmin-lab.github.io/ -->
<script type="text/javascript">
var sc_project=12455544; 
var sc_invisible=1; 
var sc_security="39ae68da"; 
</script>
<script type="text/javascript"
src="https://www.statcounter.com/counter/counter.js"
async></script>
<noscript><div class="statcounter"><a title="Web Analytics"
href="https://statcounter.com/" target="_blank"><img
class="statcounter"
src="https://c.statcounter.com/12455544/0/39ae68da/1/"
alt="Web Analytics"></a></div></noscript>
<!-- End of Statcounter Code -->


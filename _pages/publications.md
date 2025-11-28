---
title: "Kuzmin Lab - Publications"
layout: gridlay
excerpt: "Kuzmin Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Highlights

For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.com/citations?user=toi8Bz8AAAAJ&hl=en), [PubMed](https://pubmed.ncbi.nlm.nih.gov/?term=elena+kuzmin) or [Research Gate](https://www.researchgate.net/profile/Elena_Kuzmin).

For our lab code go to our [Kuzmin Lab Code github page](https://github.com/Kuzmin-Lab-code). 

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
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


## Full List

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

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

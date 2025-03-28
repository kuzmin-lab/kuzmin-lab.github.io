---
title: "Kuzmin Lab - Team"
layout: gridlay
excerpt: "Kuzmin Lab: Team members"
sitemap: false
permalink: /team/
---

# Lab Members

The lab is looking for a diverse group of people interested in functional genomics and synthetic biology. We are looking to recruit graduate students and postdocs with backgrounds in genetics, molecular biology, genomics, bioengineering, bioinformatics and computer science. Undergraduate thesis and summer students are welcome to apply!

Students are encouraged to apply through Concordia University's [Department of Biology](https://www.concordia.ca/artsci/biology.html) or [SynBio Apps Program](https://www.concordia.ca/sgs/programs/interdisciplinary/synthetic-biology-applications.html) as well as McGill University's [Rosalind & Morris Goodman Cancer Institute](https://www.mcgill.ca/gci/), [Quantitative Life Sciences Program](https://www.mcgill.ca/qls/) and [Department of Human Genetics](https://www.mcgill.ca/humangenetics/). 

Interested applicants should send Dr. Kuzmin their transcript, CV and a brief description of their research interests.


Jump to [team](#team) or [alumni](#alumni).

## Team
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br><{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
    
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}




## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br> Now: {{ member.duration }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>
{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

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


---
title: "DSSE->Members"
layout: gridlay
excerpt: "DSSE -- Members"
sitemap: false
permalink: /members/
---

<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Head of DSSE Research Group</h2>
<br>
<div class="row">
  <div class="col-sm-3 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/group-members/current_members/kazi-sakib.png" class="img-responsive" width="80%" style="float: center" />
  <br>
  <h4><a href="http://www.iit.du.ac.bd/about_iit/individual_teacher/47" target="_blank">Dr. Kazi Muheymin-Us-Sakib</a></h4>
  Professor<br>
  University of Dhaka<br>
  <i><sakib@iit.du.ac.bd></i><br>
  BSc(DU), MSc(DU), PhD(RMIT)<br>
  <a href="https://scholar.google.com/citations?user=G88J0-EAAAAJ&hl=en" target="_blank"><img src="{{ site.url }}{{ site.baseurl }}/images/logo/scholar.png" width="40px" height="40x"></a>
  <a href="http://dblp.uni-trier.de/pers/hd/s/Sakib:Kazi" target="_blank"><img src="{{ site.url }}{{ site.baseurl }}/images/logo/dblp.png" width="40px" height="40x"></a>
  <a href="http://www.researchgate.net/profile/Kazi_Sakib" target="_blank"><img src="{{ site.url }}{{ site.baseurl }}/images/logo/researchgate.png" width="40px" height="40x"></a>
  </div>
  <div class="col-sm-9"> 
  <p align="justify">
<b>Dr. Kazi Muheymin-Us-Sakib</b> is a Professor at the <a href="http://www.iit.du.ac.bd/about_iit/individual_teacher/47" target="_blank"> Institute of Information Technology (IIT)</a>, <a href="http://du.ac.bd/" target="_blank"> University of Dhaka </a>. He completed his Ph.D. at <a  href="https://www.rmit.edu.au/" target="_blank">RMIT University </a> on Distributed Systems and pursued a master's and a bachelor's degree in <a href="http://www.cse.du.ac.bd/" target="_blank"> Computer Science and Engineering (CSE)</a> at the University of Dhaka before joining as a faculty.
His research interest broadly lies in software engineering and its various aspects, for example, Adaptive and Distributed System,  Cloud Computing, Software Testing, Software Architecture & Design, Requirement Analysis, Project Management, Code Smell & Refactoring, Code Search and Code Clone. 
His work has been published in major and premier conferences & journals in the area of software engineering such as <b>ICSE, ICSME, SANER, APSEC, ENASE</b> etc. attracting substantial interest from the software engineering research community.
His research work and projects have been funded by <a href="https://ictd.gov.bd/" target="_blank">ICT Division Bangladesh </a>, <a href="https://ptd.gov.bd/" target="_blank"> Ministry of Posts, Telecommunications and Information Technology, Bangladesh </a>, <a href="http://www.ugc.gov.bd/" target="_blank"> University Grant Commission (UGC) </a> and, <a href="https://www.bdren.net.bd/" target="_blank"> Bangladesh Research and Education Network (BdREN)</a>. 
Former students of his research group have obtained Ph.D and Masters position at <b>Imperial College London</b>, Carnegie Mellon University <b>(CMU)</b>, University of Texas at Austin <b>(UT Austin)</b>, <b>NC State</b> University, University at Buffalo  <b>(SUNY)</b>, College of <b>William and Mary</b>, University of Alberta <b>(UofA)</b>, Concordia University, <b>Iowa State</b> University, University of California Santa Barbara <b>(UCSB)</b>, University of California Irvine <b>(UCI)</b>, University of Southern California <b>(USC)</b> and University College London <b>(UCL)</b>. Besides, some graduated students got employment in high-tech industries like <b>Amazon, Microsoft, Samsung, IBM</b> etc. and, secured faculty position in many prestigious and renowned public and private universities in Bangladesh, for instance, University of Dhaka <b>(DU)</b>, Shahjalal University of Science and Technology <b>(SUST)</b>, Bangladesh University of Professionals <b>(BUP)</b>, Islamic University of Technology <b>(IUT)</b>, BRAC University, Noakhali Science and Technology University<b> (NSTU)</b>, University of Barishal, Jashore University of Science and Technology <b>(JUST)</b>.</p> </div>
</div>


<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Members</h2>
<br>

{% assign number_printed = 0 %}
{% for member in site.data.members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/group-members/current_members/{{ member.photo }}"  width="128px" height="128px" style="float: left" />
  <h4><a href="{{ member.homepage }}" target="_blank">{{ member.name }}</a></h4>
  <i><b>{{ member.current_position }}</b></i> <br>
  <i><b>{{ member.current_organization }}</b></i> <br>
  <i>email: {{ member.email }}</i>
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



<!-- PhD Students  -->

<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">PhD Students</h2>
<br>

{% assign number_printed = 0 %}
{% for member in site.data.phd %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/group-members/phd/{{ member.photo }}"  width="128px" height="128px" style="float: left" />
  <h4><a href="{{ member.homepage }}" target="_blank">{{ member.name }}</a></h4>
  <i>{{ member.current_position }} </i> <br>
  <i>{{ member.current_organization }} </i> <br>
  <i>email: {{ member.email }}</i>
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

<!-- PhD Students -->

<!-- M.Phil Students  -->

<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">M.Phil Students</h2>
<br>

{% assign number_printed = 0 %}
{% for member in site.data.mphil %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/group-members/mphil/{{ member.photo }}"  width="128px" height="128px" style="float: left" />
  <h4><a href="{{ member.homepage }}" target="_blank">{{ member.name }}</a></h4>
  <i>{{ member.current_position }} </i> <br>
  <i>{{ member.current_organization }} </i> <br>
  <i>email: {{ member.email }}</i>
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

<!-- M.Phil Students -->

<!-- Alumni -->
<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Alumni</h2>
<br>

{% assign number_printed = 0 %}
{% for member in site.data.alumni %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/group-members/alumni/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{ member.homepage }}" target="_blank">{{ member.name }}</a></h4>
  <i>{{ member.current_position }} </i> <br>
  <i>{{ member.current_organization }} </i> <br>
  <i>email: {{ member.email }}</i>
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

<!-- Alumni -->




### Administrative Support
If you need to update your information, feel free to contact <a href="https://mrhmisu.github.io/" target="_blank">Md Rakib Hossain (Misu)</a>.
<br>
<br>
<br>
<style>
  @media (max-width: 420px) {.fa-ul::before{content: "\A";white-space: pre;}}
</style>
---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---


<h1 class="headline_text"> About Me </h1>
<div class="container">
	<div class="container_left">
	I am <i>Ahmad Babaeian Jelodar</i>, a PhD candidate of <a class="light_red" href="https://www.cse.usf.edu/~yusun/"> Professor Yu Sun </a> at the <a class="light_red" href="https://rpal.cse.usf.edu/"> Robot Perception and Action Lab (RPAL)</a> in the Department of Computer Science and Engineering at University of South Flordia. My research is mainly focused on deep learning applications. I have been in the PhD program since 2016 and I am expected to graduate by May 2021.
	</div> 
	<div class="container_middle">
	<p class="small_bottom_margin"> Email:</p>
	<p> ajelodar<r class="places">[at]</r>usf<r class="places">[dot]</r>edu, ahmadbab<r class="places">[at]</r>gmail<r class="places">[dot]</r>com </p>
	<p> <a href="https://www.linkedin.com/in/ahmad-babaeian-jelodar-0899aa71/"> LinkedIn </a> </p>	
	<p> <a href="https://github.com/abjelodar"> Github </a> </p>
	</div> 

	<div class="container_right">
	    <img src="assets/images/me.jpg">
	</div>
</div>


<h1 class="headline_text"> <a id="id_research"></a> Research </h1>
<p class="li_style"> My research interests include computer vision, deep learning, image processing, machine learning, and robotics. I am currently working on a project funded by NSF which the aim is to ultimately research and develop to build an autonomus robotic cooking chef. In this regard I work on identifying task graphs from images and extracting understanding from videos. </p>



<h1 class="headline_text"> <a id="id_publications"></a> Selected Publications </h1>
<ol>
{% for member in site.data.publications %}
  <li class="li_style">
      {{ member.authors }}, {{ member.title }}, {{ member.conference }}, {{ member.date }} <a href="{{ member.link }}"> (pdf)</a>.
  </li>
{% endfor %}
</ol>


<h1 id="id_education" class="headline_text"> <a id="id_education"></a> Education </h1>

<ul>
{% for member in site.data.education %}
  <li class="li_style">
	<b>{{ member.degree }}</b>, {{ member.course }}, <i class="places"> {{ member.university }}</i>, {{ member.location }}, {{ member.end_date }}.
	<ul>
		<li class="small_text"> {{ member.thesis }} </li>
	</ul>

  </li>
{% endfor %}
</ul>


<h1 id="id_experience" class="headline_text"> <a id="id_experience"></a> Work Experience </h1>
<ul>
{% for member in site.data.experience %}
  <li class="li_style">
	<b>{{ member.name }}</b>, <i class="places"> {{ member.company }}</i> , {{ member.time }}, {{ member.location }}.
	<ul>
		<li class="small_text"> {{ member.content }} </li>
	</ul>
  </li>
{% endfor %}
</ul>


<h1 id="id_posters" class="headline_text"> <a id="id_posters"></a> Talks and Posters </h1>
<ul>
{% for member in site.data.talks %}
  <li class="li_style">
	<b>{{ member.title }}</b>, {{ member.name }}, {{ member.entity }}.
	<ul>
		<li class="small_text"> {{ member.date }}, {{ member.location }}. </li>
	</ul>
  </li>
{% endfor %}
</ul>


<h1 id="id_project" class="headline_text"> <a id="id_project"></a> Projects </h1>
<ul>
{% for member in site.data.projects %}
  <li class="li_style">
	<b>{{ member.project }}</b>, {{ member.tool }}, {{ member.date }}.
	<ul>
		<li class="small_text"> {{ member.description }} <a href="{{ member.link }}">{{ member.link }}</a>. </li>
	</ul>
  </li>
{% endfor %}
</ul>


<h1 id="id_teaching" class="headline_text"> <a id="id_teaching"></a> Teaching </h1>
<ul>
{% for member in site.data.teaching %}
  <li class="li_style">
	{{ member.name }}, <b>Graduate courses</b>: <i class="places">{{ member.graduate_courses }}</i>, Undergraduate: {{ member.undergraduate_courses }}.
	<ul>
		<li class="small_text"> {{ member.location }}. </li>
	</ul>
  </li>
{% endfor %}
</ul>


<h1 id="id_awards" class="headline_text"> <a id="id_awards"></a> Awards and Memberships </h1>
<ul>
{% for member in site.data.awards_memberships %}
  <li class="li_style">
        {{member.description}}, {{member.date}}.
  </li>
{% endfor %}
</ul>


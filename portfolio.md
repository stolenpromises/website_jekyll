---
layout: project
title: Portfolio
collections: projects

---
<!-- Section -->
<section>
	<div class="posts">
	</div>
</section>

{% for project in site.projects %}
  <h2>{{ project.title }} - {{ project.filename }}{{ project.ext}}</h2>
  <p>{{ project.blurb}}</p>
{% endfor %}

<!--project list-->
<!-- 6.00.2x -->
<!-- optimization_cows-->
<!-- model-training_climate-->
<!-- sim-with-histogram-plots -->
<!-- monte-carlo_ball-draw -->
<!-- optimization-brute_array -->


<!-- 6.00.1x -->
<!-- w5_ps6 decryption -->
<!-- w4_ps4a scrabble -->
<!-- w3_ps3_hangman -->
<!-- w2_ps2_p3 credit card balance -->
<!-- misc exercizes -->
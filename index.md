---
layout: default
subtitle: Home
---
<!-- Skills -->
<section>
	<header class="major">
		<h2>Skills</h2>
	</header>
	<!-- Selection of highlighted skills. _skills collection is looped over. If a skill is marked to be included, a skill_include is called with scope of .skill variables(passed from the skill). --> 
	<div class="features">
		<!-- TODO update blubs-->
		{% for skill in site.skills %} 	{% comment %}
										loop over _collection
										{% endcomment %}
			{% if skill.highlight %}  		{% comment %}
											only iterate over highlights
											{% endcomment %}
		{% include skill.md %}			{% comment %}
										_skill variables are passed to skill.md before generation
										{% endcomment %}
			{% endif %}
		{% endfor %}
	</div>
	<div>
		<article>
			<a href="#" class="button">More skills</a>  #TODO construct
		</article>
	</div>
</section>
<!-- Projects -->
<section>
	<header class="major">
		<h2>Project Highlights</h2>
	</header>
	<!-- Selection of highlighted projects. _projects collection is looped over. If a project is marked to be included, an article _include is called with scope of .project variables(passed from the project). --> 
	<div class="posts">
		<!-- TODO update blubs-->
		{% for project in site.projects %} 	{% comment %}
											loop over _projects collection 
	 										{% endcomment %}
			{% if project.highlight %}  		{% comment %}
												only iterate over highlights 
	 											{% endcomment %}
				{% include article.html %}			{% comment %}
													_project variables are passed to article.html before generation
													{% endcomment %}
			{% endif %}
		{% endfor %}
	</div>
	<div>
		<article>
			<a href="#" class="button">More Projects</a>
		</article>
	</div>
</section>

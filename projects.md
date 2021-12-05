---
layout: default
title: Projects

---
<!-- projects -->
<section>
	<header class="major">
		<h2>Projects</h2>
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
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
				{% include article.html %}			{% comment %}
													_project variables are passed to article.html before generation
													{% endcomment %}
		{% endfor %}
	</div>
  <div>
		<ul class="actions">
        <li><a href="{{'/skills.html' |  relative_url }}" class="button">Filter Projects</a></li>
    </ul>
	</div>
</section>
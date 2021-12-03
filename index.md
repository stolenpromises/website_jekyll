---
layout: default
subtitle: Home
---
<!-- Section -->
<section>
	<header class="major">
		<h2>Skills</h2>
	</header>
	<div class="features">
		<article>
			<a href="{{ site.python_url }}"><span class="image fit"><img src="{{ site.python_svg }}" alt="" /></span></a>
			<div class="content">
				<h3>Python</h3>
				<p>I am proficient in Python</p>
			</div>
		</article>
		<article>
			<a href="{{ site.numpy_url }}"><span class="image fit"><img src="{{ site.numpy_svg }}" alt="" /></span></a>
			<div class="content">
				<h3>NumPy</h3>
				<p>I am proficient in NumPy</p>
			</div>
		</article>		
		<article>
			<a href="{{ site.github_url }}"><span class="image fit"><img src="{{ site.github_svg }}" alt="" /></span></a>
			<div class="content">
				<h3>GitHub</h3>
				<p>I am proficient in GitHub</p>
			</div>
		</article>
		<article>
			<a href="{{ site.spyder_url }}"><span class="image fit"><img src="{{ site.spyder_svg }}" alt="" /></span></a>
			<div class="content">
				<h3>Spyder IDE</h3>
				<p>I am proficient in Spyder IDE</p>
			</div>
		</article>
		<article>
			<a href="#" class="button">more skills</a>
		</article>
	</div>
</section>
<!-- Section -->
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
												only iterate over highlight projects 
	 											{% endcomment %}
				{% include article.html %}			{% comment %}
													_project variables are passed to article.html before generation
													{% endcomment %}
			{% endif %}
		{% endfor %}
	</div>
		<article>
		<a href="#" class="button">All Projects</a>
		</article>
</section>

<!-- Section -->
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
												only iterate over highlight projects 
	 											{% endcomment %}
				{% include article.html %}			{% comment %}
													_project variables are passed to article.html before generation
													{% endcomment %}
			{% endif %}
		{% endfor %}
	</div>
		<article>
		<a href="#" class="button">All Projects</a>
		</article>
</section>

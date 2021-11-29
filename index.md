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
			<a href="#" class="button">More</a>
		</article>
	</div>
</section>

<!-- Section -->
<section>
	<header class="major">
		<h2>Projects</h2>
	</header>
	<!-- selection of key projects --> 
	<div class="posts">
		<!-- TODO update blubs-->
		{% include project.html project_title="Viral Growth" filename="viral_growth" ext=".jpg" project_blurb="Simulations of viral growth within a patient under various different circumstances." %}
		{% include project.html project_title="Robot Vacuum" filename="robot" ext=".jpg" project_blurb="Random robots demonstrate algorithmic efficiency." %}
		{% include project.html project_title="This Website" filename="this_website" ext=".jpg" project_blurb="I started with an HTML5 template built for Jekyll." %}
		{% for project in site.projects %}
			{% include article.html %}
		{% endfor %}
	</div>
		<article>
		<a href="#" class="button">Full portfolio</a>
		</article>
</section>

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
	<div class="posts">
		<article>
			<a href="{{ 'portfolio/robot_vacuum.html' | absolute_url }}" class="image"><img src="{{ site.robot_jpg }}" alt="" /></a>
			<h3>Robot Vacuum</h3>
			<p>Random robots demonstrate algorithmic efficiency.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>
		<article>
			<a href="{{ 'portfolio/viral_growth.html' | absolute_url }}" class="image"><img src="{{ site.virus_jpg }}" alt="" /></a>
			<h3>Viral Growth</h3>
			<p>Simulations of viral growth within a patient under various different circumstances.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>
		<article>
			<a href="{{ 'portfolio/this_website.html' | absolute_url }}" class="image"><img src="{{ site.this_website_jpg }}" alt="" /></a>
			<h3>This website</h3>
			<p>I started with an HTML5 template built for Jekyll.</p>
			<ul class="actions">
				<li><a href="{{ 'portfolio/this_website.html' | absolute_url }}" class="button">More</a></li>
			</ul>
		</article>
	</div>
</section>

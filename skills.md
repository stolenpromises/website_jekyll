---
layout: default
title: Skills
---
<!-- skills -->
<section>
	<!-- Selection of highlighted skills. _skills collection is looped over. If a skill is marked to be included, a skill_include is called with scope of .skill variables(passed from the skill). --> 
    <div class="features">
        <!-- TODO update blubs-->
        {% for skill in site.skills %} 	{% comment %}
                                        loop over _collection
                                        {% endcomment %}
        {% include skill.md %}			{% comment %}
                                        _skill variables are passed to skill.md before generation
                                        {% endcomment %}
        {% endfor %}
    </div>
    <div>
        <ul class="actions">
            <li><a href="{{'/projects.html' |  relative_url }}" class="button">All Projects</a></li>
        </ul>
    </div>
</section>
{% comment %}
This include generates an article. It requires passage of variables from the _skills collection and searches for projects which feature that skill.
{% endcomment %}
{% comment %}
<!-- skill is {{ skill.title }}-->
{% endcomment %}
<article>
    <a href="{{ skill.attribution_url }}"><span class="image fit"><img src="{{'skills/assets/icons/'}}{{ skill.filename }}{{ '.svg' }}" alt="" /></span></a>
    <div class="content">    
        <h3>{{ skill.title }}</h3>
        <p>{{ skill.blurb }}</p>
        {% for project in site.projects %}  {% comment %}
                                            loop over _projects collection
                                            {% endcomment %}
            {% if project.skills contains skill.filename  %}    {% comment %} if skill is found in project {% endcomment %}                          
                {% comment %} add a link to skill page {% endcomment %}
        <ul class="actions">
            <li><a href="{{'/skills/'' |  absolute_url }}{{ skill.filename }}.html" class="button small">Projects featuring this skill</a></li>
        </ul>
                {% comment %}
                break to prevent multiple buttons being generated
                {% endcomment %}
                {% break %}
            {% endif %}
        {% endfor %}
    </div>
</article>
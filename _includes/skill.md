{% comment %}
This include generates an article. It requires passage of variables from the _projects collection.
{% endcomment %}
<article>
    <a href="{{'/projects/' |  absolute_url }}{{ project.filename }}.html" class="image"><img src="{{'projects/assets/images/'}}{{ project.filename }}{{project.ext}}" alt="" /></a>
    <h3>{{ project.title }}</h3>
    <p>{{ project.blurb }}</p>
    <ul class="actions">
        <li><a href="{{'/projects/'' |  absolute_url }}{{ project.filename }}.html" class="button small">view</a></li>
    </ul>
</article>
<nav class="nav-primary" role="navigation" >
    <ul>
        {% for p in site.pages %}
            {% if p.name != "main.scss" %}
                {% if p.name != "/feed.xml" %}
                <li>
                    <a {% if p.url == page.url %}class="active"{% endif %} href="{{ site.baseurl }}{{ p.url }}">{{ p.title }}</a>
                </li>
                {% endif %}
            {% endif %}
        {% endfor %}
    </ul>
</nav>

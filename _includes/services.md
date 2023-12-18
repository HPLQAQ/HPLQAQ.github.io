{% assign show_conference = site.data.services.conference.size > 0 %}
{% assign show_journal = site.data.services.journal.size > 0 %}

{% if show_conference or show_journal %}
## Services

{% if show_conference %}
<h4 style="margin:0 10px 0;">Conference Reviewers</h4>
<ul style="margin:0 0 5px;">
  {% for link in site.data.services.conference %}
    {% if link.href and link.name %}
      <li>
        <a href="{{ link.href }}"><autocolor>{{ link.name }}</autocolor></a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
{% endif %}

{% if show_journal %}
<h4 style="margin:0 10px 0;">Journal Reviewers</h4>
<ul style="margin:0 0 20px;">
  {% for journal in site.data.services.journal %}
    {% if journal.href and journal.name %}
      <li>
        <a href="{{ journal.href }}"><autocolor>{{ journal.name }}</autocolor></a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
{% endif %}

{% endif %}

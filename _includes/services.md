## Services

<h4 style="margin:0 10px 0;">Conference Reviewers</h4>

<ul style="margin:0 0 5px;">
  {% for link in site.data.services.conference %}
    <li>
      {% if link.href and link.name %}
        <a href="{{ link.href }}"><autocolor>{{ link.name }}</autocolor></a>
      {% endif %}
    </li>
  {% endfor %}
</ul>

<h4 style="margin:0 10px 0;">Journal Reviewers</h4>

<ul style="margin:0 0 20px;">
  {% for journal in site.data.services.journal %}
    <li>
      {% if journal.href and journal.name %}
        <a href="{{ journal.href }}"><autocolor>{{ journal.name }}</autocolor></a>
      {% endif %}
    </li>
  {% endfor %}
</ul>
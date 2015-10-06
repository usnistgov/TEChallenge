---
teamId: team4
layout: page
---

{% assign team = site.data.teams[page.teamId] %}
#Team - {{ team.name }}

<br/><br/>
<ul>
{% for ideas in team.ideas %}
	<li>{{ideas.title}}</li>
{% endfor %}
</ul>
<br/><br/>

###Team Collaboration
Meeting time:

Call in information:

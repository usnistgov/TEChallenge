---
title: TE Challenge Community
layout: page
---
#Community
The purpose of this page is to allow visitors and participants to see what teams are doing and how you might be involved. We expect that as you review the overviews of participant interests and team goals, you may see the makings of a new team. Please see below for how to suggest a new team effort. Comments and ideas are all welcome. 

## Project Teams
Information regarding the teams formed during (or since) the September kickoff is posted here. Organizations that have registered to participate in the Challenge may or may not be committed (yet) to a team. We expect that more teams will be formed in the coming months as other organizations hear about the Challenge and want to join. Organizations may participate in more than one team. Collaborators are welcome to join any team.  
 
###Current teams:

<table id="teams" style="width:100%">
	{% for teams in site.data.teams %}
	<tr><td colspan="3"><br/></td></tr>
	<tr>
		<td class="team" style="width:25%;text-align:center;">
			<img class="logo" src="{{ site.baseurl }}/{{ teams[1].imageUrl }}" alt="TE Challenge">
		</td>
		<td class="desc,team" style="width:50%;padding:5px;vertical-align:top;">
			<b>{{teams[1].name}}</b>
			<br/><br/>
			<ul>
			{% for ideas in teams[1].ideas %}
				<li>{{ideas.title}}</li>
			{% endfor %}
			</ul>
			<br/><br/>
			<b>What's next:</b>
			<ul style="list-style-type: none;">
				<li>Download project workseet <a href="{{teams[1].worksheetUrl}}">HERE</a></li>
				<li>Get connected with the team <a href="{{teams[1].url}}">HERE</a></li>
			</ul>
		</td> 
		<td class="team" style="width:25%;text-align:right;">
			<b>Team lead</b>
			<br/>
			{{teams[1].lead}}
			<br/><br/>
			<b>Partners</b>
			<br/>
			{% for partners in teams[1].partners %}
				{{partners.name}}<br/>
			{% endfor %}
			<br/>
		</td>
	</tr>
	{% endfor %}
</table>

##Participants
A participating organization is one that has joined (communicated required information via the Join page, and also participating in some team effort). Participant names are followed by short summaries of participant interests in the Challenge, and pdf links (when available) introduce the organization ideas and experience relative to the Challenge. Perhaps there is another organization with interests similar to yours and a team effort can be formed around that mutual interest to advance TE and the goals of the TE Challenge. 

<ul>
	{% for partner in site.data.partners %}
    <li>
		<a href="{{ partner.url }}" target="_blank">{{ partner.name }}</a> <a href="{{ partner.introdoc-url }}" target="_blank">[pdf]</a> -- {{ partner.SummaryofInterest }}
	</li>
	{% endfor %}
</ul>

##Have an idea for a new team, comment, or something else to share with us?

###>[Let us know](../join)<
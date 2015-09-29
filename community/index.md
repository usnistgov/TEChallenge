---
title: TE Challenge Community
layout: page
---
#Community

## Project Teams
Information regarding the teams formed during the September kickoff is posted here. Organizations that have registered to participate in the Challenge
may or may not be committed (yet) to a team. Some organizations might participate in more than one team. Many teams will come 
together at the Kickoff meeting. Some teams will be formed after the Kickoff as other organizations hear about the Challenge 
or some team and want to join. Collaborators are welcome to join any team.  
 
###Current teams:

<table id="teams1" style="width:100%">
	{% for teams in site.data.teams %}
	<tr><td colspan="3"><br/></td></tr>
	<tr>
		<td style="width:25%;text-align:center;">
			<img class="logo" src="{{ site.baseurl }}/{{ teams.imageUrl }}" alt="TE Challenge">
		</td>
		<td class="desc" style="width:50%;padding:5px;">
			<b>{{teams.name}}</b>
			<br/><br/>
			{{teams.plans}}
			<br/><br/>
			<b>What's next:</b>
			<ul style="list-style-type: none;">
				<li>Download project workseet <a href="{{teams.worksheetUrl}}">HERE</a></li>
				<li>Visit the project page <a href="{{teams.url}}">HERE</a></li>
			</ul>
		</td> 
		<td style="width:25%;text-align:right;">
			<b>lead</b>
			<br/>
			{{teams.lead}}
			<br/><br/>
			<b>partners</b>
			<br/>
			{% for partners in teams.partners %}
				{{partners.name}}<br/>
			{% endfor %}
			<br/><br/>
			<b>point of contact</b>
			<br/>
			TBD
		</td>
	</tr>
	{% endfor %}
</table>

###Other possible topics:

 * Interoperable Co-simulation platform to serve TE
 * Open-source TE protocols (developing code-base for Energy Interoperation transactive services)
 * TEMIX reference implementation 
 * Detailed modeling scenarios for TE
 * Economic Models for TE
 * Transactive Controls Approach and demonstration

##Want to join one of these efforts?

Here is the process to do it:

1. step 1
2. step 2
3. step 3

[Let us know](../join)

##Want to start a new project/team?

Here is the process to do it:

1. step 1
2. step 2
3. step 3

[Let us know](../join)

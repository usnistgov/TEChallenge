---
title: TE Challenge Community
layout: page
---
#Community

## Project Teams
Information regarding the teams formed during the September kickoff is posted here. Organizations that have registered to participate in the Challenge
may or may not be committed (yet) to a team. Organizations may participate in more than one team. Collaborators are welcome to join any team.  
 
###Current teams:

<table id="teams" style="width:100%">
	{% for teams in site.data.teams %}
	<tr><td colspan="3"><br/></td></tr>
	<tr>
		<td class="team" style="width:25%;text-align:center;">
			<img class="logo" src="{{ site.baseurl }}/{{ teams.imageUrl }}" alt="TE Challenge">
		</td>
		<td class="desc,team" style="width:50%;padding:5px;vertical-align:top;">
			<b>{{teams.name}}</b>
			<br/><br/>
			<ul>
			{% for ideas in teams.ideas %}
				<li>{{ideas.title}}</li>
			{% endfor %}
			</ul>
			<br/><br/>
			<b>What's next:</b>
			<ul style="list-style-type: none;">
				<li>Download project workseet <a href="{{teams.worksheetUrl}}">HERE</a></li>
				<li>Visit the project page <a href="{{teams.url}}">HERE</a></li>
			</ul>
		</td> 
		<td class="team" style="width:25%;text-align:right;">
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
 * Microgrids/Microgrid simulations – TeMIX/Microgrid applications
 * Transition from centralized to decentralized energy simulation
 * Cost management/business models/TE tariffs
 * Co-simulation platforms / simulate independent systems
 * Reference grids and scenarios
 * Simulation architecture/Architecture/frameworks (PNNL, EEI, DSO, etc.) and validation and verification of TE algorithms
 * TE interoperability
 * Power matcher/vehicles, etc.


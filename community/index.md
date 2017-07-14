---
title: TE Challenge Community
layout: page
---
# Community
The purpose of this page is to allow visitors and participants to see what teams are doing and how you might be involved. We expect that as you review the overviews of participant teams and their plans, you may consider how to cooperate with an existing team or start a new team. Comments and ideas are all welcome. 

## Phase II Project Teams
Phase II officially launched on April 20 and Phase II teams will be updated as they join or are formed. 
Organizations may participate in more than one team. Collaborators may be welcome to join an existing team.

### Pacific Northwest National Laboratory (PNNL)
<li>Introduction to Team project <a href="https://s3.amazonaws.com/nist-sgcps/TEChallenge/Library/teams/PNNL-TEC2-intro.pdf">HERE</a></li>
### Massachusetts Institute of Technology (MIT)
### National Renewable Energy Laboratory (NREL)
### Vanderbilt University
### Dartmouth University
### Tata Consultancy Services (TCS)
### University of Puerto Rico (UPR)


## Phase I Project Teams
Information regarding the 2016 Phase I teams is posted here. 
  
 
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
			<b>Plans and Publications</b>
			<ul style="list-style-type: none;">
				{% for document in site.data.documents %}
					{% if document.team == teams[0] %}
						{% if document.url %}
						<li>
							<a href="{{document.url}}"><span style="font-weight:bold;color:green;">{{document.name}}</span>
							{% if document.format == "html" %} (Web Page) {% endif %}
							{% if document.format == "doc" %} (Doc) {% endif %}
							{% if document.format == "pdf" %} (Pdf) {% endif %}
							</a>
						</li>
						{% endif %}
					{% endif %}
				{% endfor %}
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

## Participants
A participating organization is one that has joined (communicated required information via the Join page, and also participating in some team effort). Participant names are followed by short summaries of participant interests in the Challenge, and pdf links (when available) introduce the organization ideas and experience relative to the Challenge. Perhaps there is another organization with interests similar to yours and a team effort can be formed around that mutual interest to advance TE and the goals of the TE Challenge. 

<ul>
	{% for partner in site.data.partners %}
    <li> {{ partner.name }} - {{ partner.url }}
		<ul>
		{% for document in site.data.documents %}
			{% if document.team == partner.name %}
				{% if document.url %}
				<li>
					<a href="{{document.url}}"><span style="font-weight:bold;color:green;">{{document.name}}</span>
					{% if document.format == "html" %} (Web Page) {% endif %}
					{% if document.format == "doc" %} (Doc) {% endif %}
					{% if document.format == "pdf" %} (Pdf) {% endif %}
					</a>
				</li>
				{% endif %}
			{% endif %}
		{% endfor %}
		</ul>
		<em style="padding:5px;">{{ partner.SummaryofInterest }}</em>
	</li>
	{% endfor %}
</ul>

## Have an idea for a new team, comment, or something else to share with us?

### >><a href="mailto:TEChallenge-info@nist.gov ?subject=TEChallenge--Ideas and comments &body=Hi,%0A%0A(Please send us your ideas and comments and new team suggestions. If you want to join an existing team, then click on the info for that team to get connected, and also go to the Join page to register for the Challenge.) %0A%0AThanks,%0AYour name%0AYour phone%0AYour organization" >Let us know!</a><<

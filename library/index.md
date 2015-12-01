---
title: Transactive Energy Library
layout: page
---
#Library

---
<h2>Transactive Energy Library</h2>
<p>The following documents provide background on Transactive Energy</p>
<section>

<a href="#video">Videos</a> || <a href="#presentation">Presentations</a> || <a href="#document">Documents</a> || <a href="#TEapproach">TE Approaches</a> || <a href="#standard">Standards</a>
<hr />

<a id="presentation">&nbsp;</a>
<h3>TE Presentations</h3>
<dl>
{% for document in site.data.documents %}

  {% if document.category == "presentation" %}
  <dt>
  
    {% if document.url %}
        <a href="{{document.url}}"><span style="font-weight:bold;color:green;">{{document.name}}</span>
          {% if document.format == "html" %} (Web Page) {% endif %}
          {% if document.format == "doc" %} (Doc) {% endif %}
          {% if document.format == "pdf" %} (Pdf) {% endif %}
        </a>
    {% endif %}

  </dt>


  <dd>{{document.description}}</dd>

{% endif %}
{% endfor %}
</dl>

<a id="document">&nbsp;</a>
<h3>TE Documents</h3>
<dl>
{% for document in site.data.documents %}

  {% if document.category == "document" %}
  <dt>
  
    {% if document.url %}
        <a href="{{document.url}}"><span style="font-weight:bold;color:green;">{{document.name}}</span>
          {% if document.format == "html" %} (Web Page) {% endif %}
          {% if document.format == "doc" %} (Doc) {% endif %}
          {% if document.format == "pdf" %} (Pdf) {% endif %}
        </a>  
    {% endif %}
    
  </dt>


  <dd>{{document.description}}</dd>

{% endif %}
{% endfor %}
</dl>


<a id="TEapproach">&nbsp;</a>
<h3>TE Approaches</h3>
<dl>
{% for document in site.data.documents %}

  {% if document.category == "TEapproach" %}
  <dt>
    {% if document.url %}
        <a href="{{document.url}}"><span style="font-weight:bold;color:green;">{{document.name}}</span>
          {% if document.format == "html" %} (Web Page) {% endif %}
          {% if document.format == "doc" %} (Doc) {% endif %}
          {% if document.format == "pdf" %} (Pdf) {% endif %}
        </a>  
    {% endif %}
    
  </dt>


  <dd>{{document.description}}</dd>

{% endif %}
{% endfor %}
</dl>




  

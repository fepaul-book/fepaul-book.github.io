---
layout: page
title: study
permalink: /study/
description: Overview of my academic career.
nav: true
nav_order: 2
display_categories: [degrees]
horizontal: false
---

As mentioned in my CV, I have several degrees. 
This page is intended to provide an overview of my various qualifications and categorise my achievements.

General information has to be added. 
number of semesters
average cp per semester
summed cp - show how much I did more
all finished in first attempt
number of lectures per subject


Neben ersten wichtigen Kontakten bringt ein praktischer Ausflug in die Berufswelt noch mehr: Soft Skills wie Team- und Kommunikationsfähigkeit sowie Belastbarkeit können dabei erworben werden. Die wohl wichtigste fachfremde Eigenschaft für Informatiker ist die Fähigkeit zur Selbstorganisation und zum Zeitmanagement. Ein ausgeprägtes Kunden- und Dienstleistungsbewusstsein sowie mindestens englische Fremdsprachenkenntnisse runden das Profil ab.

Auch die Bereitschaft zur ständigen Weiterbildung ist für Informatikerinnen obligatorisch. Die Informatik befindet sich im ständigen Wandel: Neue Betriebssysteme werden entwickelt, der Hardware-Bereich bekommt in regelmäßigen Abständen Zuwachs und neue Programmiersprachen kommen auf den Markt. Für alle Informatikberufe gilt: Wer Erfolg haben will, für den ist lebenslanges Lernen absolute Pflicht. Eine Möglichkeit dazu ist der Besuch von Weiterbildungsmaßnahmen. Dabei wird nicht nur wichtiges Wissen erworben: Weiterbildungsmaßnahmen zeugen auch von Engagement für den Job. Sie können beispielsweise ein wichtiger Schritt sein, um sich innerhalb des Unternehmens als Führungskraft zu empfehlen. 


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/veranstaltungen.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/credits.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
	to be continued ...
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0"> <!-- Changed from col-sm-4 to col-sm-8 -->
        {% include figure.html path="assets/img/noten.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    to be continued ...
</div>


<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>

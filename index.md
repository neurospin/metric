---
layout: page_lab
---

{% assign lab = "metric" %}
{% assign teams_sorted = site.labs | where: "cat", lab | where: "subcat", "team" | sort: "title"  %}
{% assign cells_sorted = site.labs | where: "cat", lab | where: "subcat", "cell" | sort: "title"  %}

<!-- Banner -->
<section id="banner">
<div class="content" style="width: 100%;">
  <p>
  The METRIC (MEthodology and insTrumentation for human and non-human pRimate ultra-hIgh field magnetiC resonance imaging – Méthodologie Pour la Recherche en Imagerie Clinique) laboratory is part of the <a href="https://baobab.neurospin.fr/" target="_blank">BAOBAB</a> (<a href="https://www.cea.fr/english" target="_blank">CEA</a>, <a href="https://www.cnrs.fr/en" target="_blank">CNRS</a>, <a href="https://www.universite-paris-saclay.fr/en" target="_blank">Paris-Saclay University</a>) Unit in the <a href="https://joliot.cea.fr/drf/joliot/en/Pages/research_entities/NeuroSpin.aspx"  target="_blank">NeuroSpin</a> department. <br/><br/>
  <b>General view on METRIC:</b> The METRIC laboratory dedicates itself to leveraging the potential of ultra-high field MRI scanners by tackling fundamental physics problems: RF field inhomogeneity, static field (B0) inhomogeneity, SAR and temperature control, motion, field fluctuations, gradient-magnet interactions and fast and efficient MR acquisitions (anatomical, functional). We thrive on the challenge of making MRI at ultra-high field powerful and accessible to the neuroscience and medical communities to address important questions related to neurodegenerative diseases, psychiatry and cognitive sciences.  
  </p>
</div>
<div class="">
  <img src="{{site.url}}{{site.baseurl}}/images/banner.png" alt="" style="
    width: 100%;
    height: auto;
    margin-bottom: 2em;
  "/>
</div>
</section>

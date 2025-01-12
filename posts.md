---
layout: page
title: "Team"
permalink: /team/
main_nav: true
---



<div style=" border: 1px solid #ddd; border-radius: 10px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); width: 100%;margin: 20px 0;padding: 20px; position: relative; box-sizing: border-box;">     
  <img src="/website/assets/franzi.jpg" alt="Image description" style="width: 150px; height: 150px; object-fit: cover; position: absolute; top: 10px; left: 10px;">
  <div style="margin-left: 180px; text-align: left;">
    <a href = "https://franziska-boenisch.de" style=" font-size: 25px; margin-bottom: 10px;">Dr. Franziska Boenisch</a>
    <p style="font-size: 16px; color: #555;">
      Franziska ist Tenure-Track-Professorin am CISPA Helmholtz-Zentrum für Informationssicherheit, wo sie das SprintML Lab co-leitet. Zuvor war sie Postdoctoral Fellow an der University of Toronto und dem Vector Institute unter der Betreuung von Prof. Nicolas Papernot. Ihre aktuelle Forschung konzentriert sich auf Privacy-Preserving und Trustworthy Machine Learning. Franziska promovierte am Fachbereich Informatik der Freien Universität Berlin, wo sie das Konzept der Individualized Privacy in Machine Learning prägte. Während ihrer Promotion war sie wissenschaftliche Mitarbeiterin am Fraunhofer-Institut für Angewandte und Integrierte Sicherheit (AISEC), Deutschland. Sie erhielt ein Fraunhofer TALENTA-Stipendium für herausragende Nachwuchswissenschaftlerinnen, den Preis der Deutschen Industrieforschungsgesellschaft für ihre Forschung zu Privacy in Machine Learning und den Fraunhofer ICT Dissertationspreis 2023, und wurde 2024 zur GI-Junior-Fellow ernannt.
    </p>    
  </div>
</div>

<div style=" border: 1px solid #ddd; border-radius: 10px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); width: 100%;margin: 20px 0;padding: 20px; position: relative; box-sizing: border-box;">     
  <img src="/website/assets/adam.jpg" alt="Image description" style="width: 150px; height: 150px; object-fit: cover; position: absolute; top: 10px; left: 10px;">
  <div style="margin-left: 180px; text-align: left;">
    <a href = "https://adam-dziedzic.com/" style=" font-size: 25px; margin-bottom: 10px;">Dr. Adam Dziedzic</a>
    <p style="font-size: 16px; color: #555;">
      Adam ist Tenure-Track-Professor am CISPA Helmholtz-Zentrum für Informationssicherheit und co-leitet der SprintML Group. Seine Forschung konzentriert sich auf Secure und Trustworthy Machine Learning as a Service (MLaaS). Adam entwickelt Robust und Reliable Machine Learning Methods für Training und Inference von ML-Models unter Wahrung der Data Privacy und Model Confidentiality. Er war Postdoctoral Fellow am Vector Institute und der University of Toronto sowie Mitglied des CleverHans Lab unter der Betreuung von Prof. Nicolas Papernot. Seine Promotion absolvierte er an der University of Chicago, betreut von Prof. Sanjay Krishnan, wo er an Input und Model Compression für Adaptive und Robust Neural Networks arbeitete. Adam erhielt seinen Bachelor- und Master-Abschluss von der Technischen Universität Warschau in Polen. Er studierte auch an der DTU (Technische Universität Dänemark) und forschte an der EPFL, Schweiz. Adam arbeitete zudem bei CERN (Genf, Schweiz), Barclays Investment Bank in London (UK), Microsoft Research (Redmond, USA) und Google (Madison, USA).
    </p>    
  </div>
</div>



{% for category in site.categories %}
  {% capture cat %}{{ category | first }}{% endcapture %}
  <h2 id="{{cat}}">{{ cat | capitalize }}</h2>
  {% for desc in site.descriptions %}
    {% if desc.cat == cat %}
      <p class="desc"><em>{{ desc.desc }}</em></p>
    {% endif %}
  {% endfor %}
  <ul class="posts-list">
  {% for post in site.categories[cat] %}
    <li>
      <strong>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </strong>
      <span class="post-date">- {{ post.date | date_to_long_string }}</span>
    </li>
  {% endfor %}
  </ul>
  {% if forloop.last == false %}<hr>{% endif %}
{% endfor %}
<br>

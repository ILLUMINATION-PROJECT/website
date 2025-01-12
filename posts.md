---
layout: page
title: "Team"
permalink: /team/
main_nav: true
---



<div style=" border: 1px solid #ddd; border-radius: 10px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); width: 100%;margin: 20px 0;padding: 20px; position: relative; box-sizing: border-box;">     
  <img src="website/assets/franzi.jpg" alt="Image description" style="width: 150px; height: 150px; object-fit: cover; position: absolute; top: 10px; left: 10px;">
  <div style="margin-left: 180px; text-align: left;">
    <a href = "https://franziska-boenisch.de" style=" font-size: 25px; margin-bottom: 10px;">Dr. Franziska Boenisch</a>
    <p style="font-size: 16px; color: #555;">
      Franziska is a tenure-track faculty at the CISPA Helmholtz Center for Information Security where she co-leads the SprintML lab. Before, she was a Postdoctoral Fellow at the University of Toronto and Vector Institute advised by Prof. Nicolas Papernot. Her current research centers around private and trustworthy machine learning. Franziska obtained her Ph.D. at the Computer Science Department at Freie University Berlin, where she pioneered the notion of individualized privacy in machine learning. During her Ph.D., Franziska was a research associate at the Fraunhofer Institute for Applied and Integrated Security (AISEC), Germany. She received a Fraunhofer TALENTA grant for outstanding female early career researchers, the German Industrial Research Foundation prize for her research on machine learning privacy, and the Fraunhofer ICT Dissertation award 2023, and was named a GI-Junior Fellow in 2024.
    </p>    
  </div>
</div>

<div style=" border: 1px solid #ddd; border-radius: 10px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); width: 100%;margin: 20px 0;padding: 20px; position: relative; box-sizing: border-box;">     
  <img src="website/assets/adam.jpg" alt="Image description" style="width: 150px; height: 150px; object-fit: cover; position: absolute; top: 10px; left: 10px;">
  <div style="margin-left: 180px; text-align: left;">
    <a href = "https://adam-dziedzic.com/" style=" font-size: 25px; margin-bottom: 10px;">Dr. Adam Dziedzic</a>
    <p style="font-size: 16px; color: #555;">
      Adam is a Tenure Track Faculty Member at CISPA Helmholtz Center for Information Security, co-leading the SprintML group. His research is focused on secure and trustworthy Machine Learning as a Service (MLaaS). Adam designs robust and reliable machine learning methods for training and inference of ML models while preserving data privacy and model confidentiality. Adam was a Postdoctoral Fellow at the Vector Institute and the University of Toronto, and a member of the CleverHans Lab, advised by Prof. Nicolas Papernot. He earned his PhD at the University of Chicago, where he was advised by Prof. Sanjay Krishnan and worked on input and model compression for adaptive and robust neural networks. Adam obtained his Bachelor's and Master's degrees from the Warsaw University of Technology in Poland. He was also studying at DTU (Technical University of Denmark) and carried out research at EPFL, Switzerland. Adam also worked at CERN (Geneva, Switzerland), Barclays Investment Bank in London (UK), Microsoft Research (Redmond, USA), and Google (Madison, USA).
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

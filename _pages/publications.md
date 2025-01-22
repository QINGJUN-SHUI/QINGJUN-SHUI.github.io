---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<!-- New style rendering if publication categories are defined -->
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  <div class="publication-entry">
    <h2>1. Evaporable Fullerene Indanones with Controlled Amorphous Morphology as Electron Transport Layers for Inverted Perovskite Solar Cells</h2>
    <p><strong>Authors:</strong> Qing-Jun Shui, Shiqi Shan, Yong-Chang Zhai, Shinobu Aoyagi, Seiichiro Izawa, Miftakhul Huda, Chu-Yang Yu, Lijian Zuo, Hongzheng Chen *, Hao-Sheng Lin *, and Yutaka Matsuo *</p>
    <p><strong>Venue:</strong> Journal of the American Chemical Society, 2023, <strong>145</strong>, 50, 27307–27315</p>
    <p><strong>Date:</strong> December 8, 2023</p>
    <p><strong>DOI:</strong> <a href="https://doi.org/10.1021/jacs.3c07192">10.1021/jacs.3c07192</a></p>
    <div class="publication-image">
      <img src="/images/FIDO.png" alt="FIDO" style="width: 100%; max-width: 600px; margin: 20px 0;" />
    </div>
    <p><a href="https://doi.org/10.1021/jacs.3c07192" class="btn btn-primary" target="_blank">Read Full Paper</a></p>
  </div>
{% endif %}



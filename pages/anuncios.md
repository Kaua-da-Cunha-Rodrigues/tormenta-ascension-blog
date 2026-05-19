---
title: Anúncios
layout: page
permalink: /anuncios/
description: Comunicados oficiais, atualizações de sistema e notícias importantes de Tormenta Ascension.
---

<div class="forum-panel">
  <div class="forum-panel__title">
    <h2>📢 Comunicados Oficiais</h2>
    <span class="badge">Sistema Tormenta</span>
  </div>
  <table class="post-table">
    <thead>
      <tr>
        <th class="col-icon"></th>
        <th class="col-title">Tópico</th>
        <th class="col-meta">Data / Autor</th>
      </tr>
    </thead>
    <tbody>
      {% assign anuncios = site.categories.anuncios %}
      {% for post in anuncios %}
        {% include post-card.html post=post %}
      {% else %}
        <tr><td colspan="3" class="empty-state">Nenhum anúncio publicado ainda.</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

---
title: Comunidade
layout: page
permalink: /comunidade/
description: Relatos de aventura, histórias de personagem, registros de guilda e postagens dos jogadores.
---

<div class="community-info">
  📜 Esta seção é escrita pelos jogadores. Poste relatos de dungeon, histórias de seu personagem, anúncios de guilda e registros de batalha como se fossem acontecimentos reais dentro de Arton.
</div>

<div class="forum-panel">
  <div class="forum-panel__title">
    <h2>🛡 Relatos da Comunidade</h2>
    <span class="badge">Jogadores</span>
  </div>
  <table class="post-table">
    <thead>
      <tr>
        <th class="col-icon"></th>
        <th class="col-title">Relato</th>
        <th class="col-meta">Data / Autor</th>
      </tr>
    </thead>
    <tbody>
      {% assign comunidade = site.categories.comunidade %}
      {% for post in comunidade %}
        {% include post-card.html post=post %}
      {% else %}
        <tr><td colspan="3" class="empty-state">Nenhum relato publicado ainda. Seja o primeiro a contar sua história!</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

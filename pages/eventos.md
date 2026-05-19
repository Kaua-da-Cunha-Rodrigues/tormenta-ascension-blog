---
title: Eventos
layout: page
permalink: /eventos/
description: Eventos especiais, chefes globais, festivais e acontecimentos temporários do servidor.
---

<div class="event-callout">
  ⚔ <strong>Evento ativo:</strong> Festival da Primeira Chama — disponível nas grandes cidades de Arton durante a primeira semana.
</div>

<div class="forum-panel">
  <div class="forum-panel__title">
    <h2>🗓 Calendário de Eventos</h2>
    <span class="badge">Temporada Atual</span>
  </div>
  <table class="post-table">
    <thead>
      <tr>
        <th class="col-icon"></th>
        <th class="col-title">Evento</th>
        <th class="col-meta">Data / Equipe</th>
      </tr>
    </thead>
    <tbody>
      {% assign eventos = site.categories.eventos %}
      {% for post in eventos %}
        {% include post-card.html post=post %}
      {% else %}
        <tr><td colspan="3" class="empty-state">Nenhum evento publicado ainda.</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

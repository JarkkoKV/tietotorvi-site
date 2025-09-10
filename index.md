---
layout: default
title: Tietotorvi – Hyvät uutiset
---

<!-- HERO -->
<section class="hero hero--with-illustration is-placed">
  <div class="wrap">
    <div class="hero_content">
      <h1>Tietotorvi – Hyvät uutiset</h1>
      <p>Tälle sivulle kootaan tutkittuun tietoon ja viranomaislähteisiin perustuvia hyviä uutisia. Tehdään tieto näkyväksi ja rakennetaan tulevaisuutta tietoon tukeutuen.</p>
      <div class="hero_cta">
        <a class="btn" href="/uutiset/">Lue uusimmat</a>
        <a class="btn btn-ghost" href="https://tietotorvi.substack.com" target="_blank" rel="noopener">Tilaa uutiskirje</a>
      </div>
    </div>
  </div>
</section>

<!-- UUSIMMAT -->
<section class="wrap" style="margin-top: 24px;">
  <h2 class="section-title">Uusimmat jutut</h2>
  <div class="post-grid">
  {% for post in site.posts limit: 6 %}
    <article class="article-card">
      <h3><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
      <div class="article-meta">
        <small>{{ post.date | date: "%d.%m.%Y" }}{% if post.categories and post.categories.size > 0 %} • {{ post.categories | join: ", " }}{% endif %}</small>
      </div>
      {% if post.excerpt %}<p>{{ post.excerpt | strip_newlines }}</p>{% endif %}
      <a class="readmore" href="{{ post.url | prepend: site.baseurl }}">Lue lisää →</a>
    </article>
  {% endfor %}
  </div>
</section>

<!-- TILAUSLAATIKKO -->
<section class="wrap" style="margin-top: 24px;">
  <div class="info">
    <strong>Haluatko hyvät uutiset sähköpostiisi?</strong>
    &nbsp;Tilaa uutiskirje: <a href="https://tietotorvi.substack.com" target="_blank" rel="noopener">tietotorvi.substack.com</a>
  </div>
</section>

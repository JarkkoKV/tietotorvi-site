---
layout: default
title: Tietotorvi – Hyvät uutiset
---

<!-- HERO -->
<div class="hero">
  <div class="hero__image">
    <img src="/assets/img/hero-bg.jpg" alt="Abstrakti tausta – Tieto näkyväksi" />
  </div>
  <div class="hero__overlay"></div>
  <div class="hero__content">
    <h1>Tietotorvi – Hyvät uutiset</h1>
    <p>Tälle sivulle kootaan tutkittuun tietoon ja viranomaislähteisiin perustuvia hyviä uutisia. Tehdään tieto näkyväksi ja rakennetaan tulevaisuutta tietoon tukeutuen.</p>
  </div>
</div>

<section class="wrap" style="margin-top: 16px;">
  <h2>Uusimmat jutut</h2>
  <ul>
    {% for post in site.posts limit:5 %}
      <li style="margin: 0 0 10px 0;">
        <a href="{{ post.url }}">{{ post.title }}</a>
        <small> · {{ post.date | date: "%d.%m.%Y" }}</small>
      </li>
    {% endfor %}
  </ul>
</section>

<section class="wrap" style="margin-top: 24px;">
  <h2>Tilaus</h2>
  <div class="card" style="margin-top: 8px;">
    Haluatko uutiset sähköpostiisi? Tilaa uutiskirje: <a href="https://tietotorvi.substack.com">tietotorvi.substack.com</a>
  </div>
</section>

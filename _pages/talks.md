---
title: "Talks"
permalink: /talks/
---

# Talks

Selected conference presentations and professional talks related to software measurement, software estimation, and COSMIC functional size measurement.


## 2026

<div class="talk-card">

  <div class="talk-card__content">
    <span class="talk-card__type">IWSM–MENSURA 2026 · Paper Presentations</span>

    <h2>A Software Version Upgrade Sized with the COSMIC ISO Standard: Management Lessons Learned from a Case Study</h2>

    <p class="talk-card__meta">
      <strong>🏆 Best Paper Award</strong><br>
      IWSM–MENSURA 2026<br>
      İzmir, Türkiye · September 2026
      
    </p>

    <h2>Sizing Software Application Generators: A Case Study of the SimSE Educational Games Generator for Software Engineering Students</h2>

    <p class="talk-card__meta">
      IWSM–MENSURA 2026<br>
      İzmir, Türkiye · September 2026
    </p>
  </div>

  <div class="talk-card__image">
    <a href="{{ '/images/talks/1iwsm-mensura-2026-papers.jpg' | relative_url }}"
       class="talk-poster-link">
      <img src="{{ '/images/talks/1iwsm-mensura-2026-papers.jpg' | relative_url }}"
           alt="Two research paper presentations at IWSM–MENSURA 2026">
    </a>
  </div>

</div>

<div class="talk-card">

  <div class="talk-card__content">
    <span class="talk-card__type">IWSM–MENSURA 2026 · Hands-on Workshop</span>

    <h2>World Première: Software Estimation Educational Games</h2>

    <p class="talk-card__meta">
      A Two-Hour Hands-on Conference Workshop<br>
      IWSM–MENSURA 2026<br>
      İzmir, Türkiye · September 2026
    </p>
  </div>

  <div class="talk-card__image">
    <a href="{{ '/images/talks/software-estimation-games-workshop.jpg' | relative_url }}"
       class="talk-poster-link">
      <img src="{{ '/images/talks/software-estimation-games-workshop.jpg' | relative_url }}"
           alt="World Première: Software Estimation Educational Games — A Two-Hour Hands-on Conference Workshop">
    </a>
  </div>

</div>


## 2024

<div class="talk-card">

  <div class="talk-card__content">
    <span class="talk-card__type">IWSM-MENSURA 2024 · Research Presentations</span>

    <h2>Challenges on Standardization of User Stories and COSMIC Sizing</h2>

    <p class="talk-card__meta">
      École de technologie supérieure (ÉTS), Montréal, Canada<br>
      September 30, 2024
    </p>
  </div>

<div class="talk-card__image">

  <a href="{{ '/images/talks/iwsm-mensura-2024.jpg' | relative_url }}"
     class="talk-poster-link">

    <img src="{{ '/images/talks/iwsm-mensura-2024.jpg' | relative_url }}"
         alt="Challenges on Standardization of User Stories and COSMIC Sizing">

  </a>

</div>

</div>

## 2020

<div class="talk-card talk-card--poster">

  <div class="talk-card__content">
    <span class="talk-card__type">APH in China · Agile CxO Launch Event</span>

    <h2>APH in China</h2>

    <p class="talk-card__meta">
      Presentation on the Chinese edition of the Agile Performance Holarchy (APH)<br>
      April 2020
    </p>
  </div>

  <div class="talk-card__image talk-card__image--poster">

    <a href="{{ '/images/talks/aph-china-2020.jpg' | relative_url }}"
       class="talk-poster-link">

      <img src="{{ '/images/talks/aph-china-2020.jpg' | relative_url }}"
           alt="APH in China presentation, April 2020">

      <span class="talk-poster-link__text">
        View Full Poster
      </span>

    </a>

  </div>

</div>



<div class="poster-lightbox" id="poster-lightbox" aria-hidden="true">
  <button class="poster-lightbox__close" type="button" aria-label="Close">
    ×
  </button>

  <img
    class="poster-lightbox__image"
    id="poster-lightbox-image"
    src=""
    alt="">
</div>

<script>
  document.querySelectorAll('.talk-poster-link').forEach(function(link) {
    link.addEventListener('click', function(event) {
      event.preventDefault();

      const lightbox = document.getElementById('poster-lightbox');
      const image = document.getElementById('poster-lightbox-image');

      image.src = this.getAttribute('href');
      image.alt = this.querySelector('img').alt;

      lightbox.classList.add('is-open');
      lightbox.setAttribute('aria-hidden', 'false');
    });
  });

  document.querySelector('.poster-lightbox__close').addEventListener('click', function() {
    const lightbox = document.getElementById('poster-lightbox');

    lightbox.classList.remove('is-open');
    lightbox.setAttribute('aria-hidden', 'true');
  });

  document.getElementById('poster-lightbox').addEventListener('click', function(event) {
    if (event.target === this) {
      this.classList.remove('is-open');
      this.setAttribute('aria-hidden', 'true');
    }
  });
</script>

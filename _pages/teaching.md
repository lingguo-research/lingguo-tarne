---
title: "Teaching & Training"
permalink: /teaching/
---

# Teaching & Training

My teaching and professional training activities focus on software measurement, COSMIC functional size measurement, software estimation, and related software engineering practices.


<h2>Professional Training</h2>

<div class="teaching-card">

  <h3>COSMIC Training</h3>

  <p>
    I have delivered professional COSMIC training to practitioners from organizations including Shanghai Stock Exchange Technology, Shanghai Futures Information Technology, PwC China, GAC Toyota, Ping An Bank, Wuhan Rural Commercial Bank, Beijing Teamsun, NSFOCUS, Ningbo Bank, and China Mobile.
  </p>

</div>


<div class="teaching-card">

  <h3>Online Courses</h3>

  <p>
    I delivered <strong>multiple online courses</strong> on software measurement and COSMIC, with more than <strong>1,000 participants</strong>.
  </p>

</div>


<div class="teaching-card">

  <h3>Online Training Programs</h3>

  <p>
    I delivered more than <strong>20 training sessions</strong> through two online training programs, reaching more than <strong>200 participants</strong>.
  </p>

</div>


<div class="teaching-card">

  <h3>Professional Course Development</h3>

  <p>
    I have also collaborated on the development and production of professional online course materials and instructional videos.
  </p>

</div>


<h2>Training Photos</h2>

<div class="training-gallery">

<figure class="training-photo training-photo--poster">

  <a href="{{ '/images/teaching/online-training-2022.jpg' | relative_url }}"
     class="training-poster-link">

    <img src="{{ '/images/teaching/online-training-2022.jpg' | relative_url }}"
         alt="Online COSMIC Training, 2022">

  </a>

  <figcaption>Online COSMIC Training, 2022</figcaption>

</figure>

  <figure class="training-photo">
    <img src="{{ '/images/teaching/training-2017.jpg' | relative_url }}"
         alt="Professional COSMIC training, 2017">
    <figcaption>Professional training, 2017</figcaption>
  </figure>

  <figure class="training-photo">
    <img src="{{ '/images/teaching/training-2016.jpg' | relative_url }}"
         alt="Internal Management Process Training, 2016">
    <figcaption>Internal Management Process Training, 2016</figcaption>
  </figure>



</div>


<h2>Selected Organizations</h2>

{% include section-clients.html %}

<div class="training-lightbox" id="training-lightbox">
  <button class="training-lightbox__close"
          type="button"
          aria-label="Close">×</button>

  <img id="training-lightbox-image"
       src=""
       alt="Online COSMIC Training, 2022">
</div>

<script>
  const posterLink = document.querySelector('.training-poster-link');
  const lightbox = document.getElementById('training-lightbox');
  const lightboxImage = document.getElementById('training-lightbox-image');
  const closeButton = document.querySelector('.training-lightbox__close');

  if (posterLink && lightbox && lightboxImage) {
    posterLink.addEventListener('click', function(event) {
      event.preventDefault();

      lightboxImage.src = posterLink.getAttribute('href');
      lightbox.classList.add('is-open');
    });

    closeButton.addEventListener('click', function() {
      lightbox.classList.remove('is-open');
    });

    lightbox.addEventListener('click', function(event) {
      if (event.target === lightbox) {
        lightbox.classList.remove('is-open');
      }
    });
  }
</script>

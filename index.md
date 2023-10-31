---
layout: default
title: Ferme de la Vauzelle
description: Agriculture biologique, Diversification, Insertion, Innovation ouverte et collaborative.
---
<div>
    <iframe 
        src="https://www.youtube.com/embed/NwYK3D_hmJY" width="100%" height="500" frameborder="0" allowfullscreen="">
    </iframe>
</div>

<link href="https://cdn.jsdelivr.net/npm/modern-normalize@v2.0.0/modern-normalize.min.css" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" crossorigin="anonymous">

# Histoire
La ferme de **La Vauzelle** faisait partie autrefois du domaine de **La Roche Courbon**.
Le **31/12/1817**, **Charlotte de Courbon** ceda le domaine de La Roche Courbon et la ferme de la Vauzelle lors d'une vente judiciaire.

<div class="row">
    {% for hi in site.data.infos %}
    <div class="col-sm-3 mb-3 mb-sm-0">
        <div class="card" style="width: 14rem;">
            <img src="{{ hi.image }}" class="card-img-top" alt="">
            <div class="card-body">
                <h5 class="card-title">{{ hi.name }}</h5>
                <p class="card-text">{{ hi.content }}</p>
            </div>
        </div>
    </div>
    {% endfor %}
</div>

# Projets

  <div id="carouselExampleCaptions" class="carousel slide">
    <div class="carousel-indicators">
      <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
      <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
      <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="/assets/img/1.jpg" class="d-block w-100" alt="">
        <div class="carousel-caption d-none d-md-block">
          <h5>Economie circulaire et solidaire</h5>
          <p>L'association 2Franc6sous propose des objets de seconde main.</p>
        </div>
      </div>
      <div class="carousel-item">
        <img src="/assets/img/2.jpg" class="d-block w-100" alt="">
        <div class="carousel-caption d-none d-md-block">
          <h5>Horticulture biologique</h5>
          <p>L'association Floricotte produit des fleurs biologiques à destination des particuliers et professionnels.</p>
        </div>
      </div>
      <div class="carousel-item">
        <img src="/assets/img/3.jpg" class="d-block w-100" alt="">
        <div class="carousel-caption d-none d-md-block">
          <h5>Nouvelle technologie</h5>
          <p>L'association OSFarm installe des équipements innovants permettant de mettre en place la géolocalisation centimétrique.</p>
        </div>
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
  <script src="https://code.jquery.com/jquery-3.7.0.min.js" crossorigin="anonymous"></script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js" crossorigin="anonymous"></script>

# Mentions légales

La ferme de La Vauzelle est la propriété de la SCI des chênes verts
[Informations juridiques](https://www.pappers.fr/entreprise/les-chenes-verts-840968499)
[Nous contacter](mailto:sci-chenes-verts@gmail.com)
---
title: Histoire
layout: home
description: "3 anneaux pour les embarquer tous"
---
<link href="https://cdn.jsdelivr.net/npm/modern-normalize@v2.0.0/modern-normalize.min.css" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" crossorigin="anonymous">

# Avant 2020

La ferme de **La Vauzelle** faisait partie autrefois du domaine de **La Roche Courbon**.
Le **31/12/1817**, **Charlotte de Courbon** ceda le domaine de La Roche Courbon et la ferme de la Vauzelle lors d'une vente judiciaire.

<div class="row">
    {% for hi in site.data.infos %}
    <div class="col-sm-2 mb-2 mb-sm-0">
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

# Depuis 2020

La gouvernance des Chênes Verts met en place progressivement sa politique d'activités **diversifiées** et **durables** autour de l'**agriculture**, de l'**innovation** et de l'**économie sociale et solidaire**.

<div class="row">
    {% for hi in site.data.recents_infos %}
    <div class="col-sm-2 mb-2 mb-sm-0">
        <div class="card" style="width: 14rem;">
            <a href="{{ hi.link }}"><img src="{{ hi.image }}"  class="card-img-top" alt=""></a>
            <div class="card-body">
                <h5 class="card-title">{{ hi.name }}</h5>
                <p class="card-text">{{ hi.content }}</p>
            </div>
        </div>
    </div>
    {% endfor %}
</div>

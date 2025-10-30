---
title: Qui sommes nous
layout: home
description: "3 anneaux pour les embarquer tous"
---

<h4 style="text-align: center;">Depuis <span class="badge bg-success">2020</span>
, la ferme de La Vauzelle est la propriété des<span class="badge bg-success">Chênes verts</span> qui est une SCI familiale composée de cousins / cousines issues de la famille JOULIN</h4>

<div class="row">
    {% for ty in site.data.associates %}
    <div class="col d-flex justify-content-center">
        <div class="card" style="width: 14rem;">
            <img src="{{ ty.image }}" class="card-img-top" alt="">
            <div class="card-body">
                <a href="{{ ty.link }}"><h5 class="card-title">{{ ty.name }}</h5></a>
                <p class="card-title">{{ ty.function }}</p>
                <p class="card-text">{{ ty.content }}</p>
            </div>
        </div>
    </div>
    {% endfor %}
</div>


<div><a class="text-center f5 mt-4 pt-4" href="https://www.pappers.fr/entreprise/les-chenes-verts-840968499" target="_blank"><span>SCI Les Chênes verts | 8, rue du bouil bleu | 17250 SAINT-PORCHAIRE</span></a></div>

<div><a class="text-center f5 mt-4 pt-4" href="mailto:sci.chenes.verts@gmail.com"><span>Contactez nous !</span></a></div>
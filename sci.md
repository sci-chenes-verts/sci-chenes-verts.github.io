---
title: Qui sommes nous
layout: home
description: "3 anneaux pour les embarquer tous"
---
<br>
<h4 style="text-align: center;">Depuis <span class="badge bg-success">2020</span>
, la ferme de La Vauzelle est la propriété des<span class="badge bg-success">Chênes verts</span> qui est une société familiale composée de profils <span class="badge bg-success">experts, atypiques et complémentaires</span></h4>
<br>
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
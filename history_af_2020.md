---
title: "Après 2020"
layout: home
description: "Après 2020"
---

# Depuis 2020

La gouvernance des Chênes Verts met en place progressivement sa politique d'activités **diversifiées** et **durables** autour de l'**agriculture**, de l'**innovation** et de l'**économie sociale et solidaire**.

<div class="album py-5 bg-light">
    <div class="container">
        <div class="row">
            {% for ty in site.data.recents_infos %}
            <div class="col-md-4">
              <div class="card shadow-sm">
                <img class="card-img-top" src="{{ ty.image }}" style="height: auto; width: auto;display: flex">
                <div class="card-body">
                  <p class="card-text">{{ ty.content }}</p>
                  <div
                    class="d-flex justify-content-between align-items-center"
                  >
                    <small class="text-body-secondary">{{ ty.year }}</small>
                  </div>
                </div>
              </div>
            </div>
            {% endfor %}
        </div>
    </div>
</div>
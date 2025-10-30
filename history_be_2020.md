---
title: "Avant 2020"
layout: home
description: "Avant 2020"
---
# Avant 2020

La ferme de **La Vauzelle** faisait partie autrefois du domaine de **La Roche Courbon**.
Le **31/12/1817**, **Charlotte de Courbon** ceda le domaine de La Roche Courbon et la ferme de la Vauzelle lors d'une vente judiciaire.

<div class="album py-5 bg-light">
    <div class="container">
        <div class="row">
            {% for ty in site.data.infos %}
            <div class="col-md-4">
              <div class="card shadow-sm">
                <img class="card-img-top" src="{{ ty.image }}" style="height: auto; width: auto;display: block;">
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
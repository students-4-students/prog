---
layout: default
title: Synchroniser
parent: "Partie 5 : Collaborer"
nav_order: 3
section: IN-SC
permalink: in-sc/collaboration/sync
---

# Synchroniser les dépôts local et distant
{: .no_toc }

Maintenant, nous allons voir ce qui rend un dépôt distant si pratique : tu peux très facilement le synchroniser avec ton dépôt local.

<figure>
  <img src="/assets/storyset-uploading.svg" alt="">
  <figcaption>Illustration par <a href="https://storyset.com" target="_blank">Storyset</a>.</figcaption>
</figure>

<hr>
## Table des matières
{: .no_toc.text-delta }
1. TOC
{:toc}
<hr>

## *Fetch* et *pull* : récupérer les modifications distantes

### *Fetch*
Pour récupérer des modifications depuis GitHub, il faut commencer par faire un ***fetch*** : cela demande à Git de s’informer des changements sur le dépôt distant. Par contre, cela ne modifie pas encore ton dépôt local : ce sera fait dans l’étape suivant, le *pull*.

À noter que GitHub Desktop fait parfois des *fetch* automatiquement, donc tu n’as pas toujours besoin de faire cette action toi-même.

Pour cela, clique sur bouton **Fetch origin** s’affiche dans la barre du haut (note : ce bouton est remplacé par le bouton *push* ou *pull* si l’une de ces actions est possible).

![Le bouton “fetch” dans GitHub Desktop](/assets/fetch.png)

### *Pull*
Une fois que tu as *fetch* des modifications, tu peux les ***pull*** : cela va les intégrer dans ta branche locale. Il suffit d’appuyer sur le bouton **Pull origin** de la barre du haut.

![Le bouton “pull” dans GitHub Desktop](/assets/pull.png)

<div class="warning">
  <header>En cas de conflit</header>
  <p>Il est possible que cette étape cause un conflit, si certains changements sur le dépôt distant interfèrent avec des changements en local. Si cela t’arrive, tu peux les résoudre comme vu dans <a href="../branches/merge">la partie précédente</a>.</p>
</div>

## *Push* : envoyer ses modifications
Enfin, lorsque tu as fait des commits en local, tu peux les envoyer sur le dépôt distant avec un ***push***. Lorsque c’est possible de le faire, GitHub Desktop affiche un bouton **Push origin** dans la barre du haut.

![Le bouton “push” dans GitHub Desktop](/assets/push.png)

<div class="warning">
  <header>Quand peut-on faire un <em>push</em> ?</header>

  <p>
    Git ne t’autorise à faire un <em>push</em> <strong>que</strong> lorsque ton dernier commit local est situé <strong>après</strong> le dernier commit sur le dépôt distant <small>(par rapport à l’ordre de succession des commits, pas par rapport à leur date)</small>.
  </p>

  <p>
    La situation contraire se produit par exemple lorsqu’une autre personne a créé des commits sur le dépôt distant depuis la dernière fois que tu as <em>pull</em>.
    Dans ce cas, il faudra que tu <em>pull</em> ces modifications avant de pouvoir <em>push</em> les tiennes.
  </p>

  <img src="/assets/push-tip.svg" alt="Schéma">

  <p>
    Mais ne te fais pas de soucis : si la situation nécessite que tu <em>pull</em> avant de <em>push</em>, GitHub Desktop affichera le bouton <em>pull</em> à la place, suivi de deux flèches qui indiquent que des modifications locales n’ont pas encore été <em>push</em>.
  </p>

  <img src="/assets/pull-push.png" alt="Bouton “pull” avec deux flèches">
</div>

<div class="note">
  <header>Publier une nouvelle branche</header>
  <p>Note que si tu travailles sur une <a href="../branches/manage#créer-une-branche">nouvelle branche</a>, GitHub Desktop affichera à la place du bouton <em>push</em> un bouton <strong>Publish branch</strong>. Il fait sensiblement la même chose, mais en plus il va créer la nouvelle branche sur le dépôt distant.</p>

  <img src="/assets/publish-branch.png" alt="Bouton “Publish branch” dans GitHub Desktop">
</div>

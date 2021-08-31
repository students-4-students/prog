---
layout: default
title: Utiliser les pull requests
parent: "Partie 5 : Collaborer"
nav_order: 3
permalink: /collaboration/pull-request
---

# Utiliser les *pull requests*
{: .no_toc }

Lors de la partie précédente, nous avons vu comment fusionner des branches. Une **pull request**[^1] permet à quelqu’un de **demander** à ce qu’une branche soit fusionnée à une autre. Cette demande s’affichera alors sur la page *Pull requests* de ton dépôt sur GitHub, et elle pourra être ensuite acceptée ou refusée.

[^1]: Pour information, la même fonctionnalité est appelée *merge request* sur GitLab.

<figure>
  <img src="../assets/storyset-pull-request.svg" alt="">
  <figcaption>Illustration par <a href="https://storyset.com" target="_blank">Storyset</a>.</figcaption>
</figure>

<hr>
## Table des matières
{: .no_toc.text-delta }
1. TOC
{:toc}
<hr>

## Les *pull requests* : pourquoi ?

Cette fonctionnalité possède de nombreux avantages par rapport à une simple fusion :

* En règle générale, **tout le monde peut créer une *pull request***, même les gens qui n’ont pas la permission de modifier le dépôt.

<div class="note indent">
  <header>Note</header>
  <p>
    La plupart des logiciels dits <em>open source</em> sont développés de cette manière : tout le monde peut voir le code source, mais seul un petit nombre de personnes de confiance peut modifier le dépôt lui-même. Par contre, il est possible de proposer des modifications en créant une <em>pull request</em> qui pourra être acceptée par l’équipe du projet. Cela permet d’accepter des contributions des quatre coins du monde, en évitant les problèmes qui pourraient apparaître si n’importe qui pouvait modifier le dépôt quand bon lui semble.
  </p>
</div>

* Chaque *pull request* a un espace de discussion pour pouvoir parler de leur avancement. On peut demander à quelqu’un de relire notre *pull request*, qui pourra alors proposer des modifications ou donner son approbation.
* Ce système offre une meilleure traçabilité des modifications effectuées sur le projet et de leur cheminement. Pour cette raison, il peut être utile d’utiliser les *pull requests* même sur des projets en solo.

## Créer une *pull request*
Tu peux débuter une *pull request* de ces deux manières :

* **Depuis GitHub Desktop**
  <br>Si tu es en train de travailler avec GitHub Desktop, et que la branche que tu veux fusionner a bien entendu déjà été publiée sur GitHub, alors il te suffit de cliquer sur le bouton *Create Pull Request* qui s’affiche sur l’écran principal[^2].

@TODO Image

[^2]: Au cas où tu aurais des modifications qui n’ont pas encore été commit dans ton projet, tu peux retrouver le même bouton dans le menu *Branch* de GitHub Desktop.

* **Depuis GitHub.com**
  <br>Rends-toi sur la page de ton projet, puis dans l’onglet *Pull requests*, et clique sur le bouton *New pull request*. Sélectionne ensuite les deux branches concernées.

@TODO Image

<div class="tip indent">
  <header>Astuce</header>
  <p>
    Lorsque tu publies une nouvelle branche sur le dépôt distant, GitHub affiche un haut de la page du dépôt un lien direct vers la création d’une nouvelle <em>pull request</em> pour cette branche.
  </p>
  <img src="../assets/quick-pr.png" alt="Capture d’écran de GitHub">
</div>

## Relire une *pull request*
@TODO

## Approuver une *pull request*
@TODO

## Notes de bas de page

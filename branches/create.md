---
layout: default
title: Nouvelle branche
parent: "Partie 4 : Branches"
nav_order: 1
permalink: /branches/create
---

# Créer une nouvelle branche

Dans cette partie nous allons découvrir comment creer une nouvelle branche. Pour ce faire nous vous montrerons trois méthodes différentes (Github-Desktop, GitHub, et grâce au bon vieux terminal)
* [Depuis GitHub-Desktop](#créer-une-branche-grâce-à-github-desktop)
* [Depuis GitHub](#créer-une-branche-grâce-à-github)
* [Depuis le Terminal](#créer-une-branche-grâce-au-terminal)

## Créer une branche grâce à Github Desktop

Une fois **Github Desktop** installé et le dépôt initialisé vous pouvez créer une nouvelle branche. Pour ce faire simplement cliquez sur le bouton correspondant. Une fenêtre s'ouvrira alors demandant le nom de cette branche. Par exemple `hotfix-feature-tchu`.

![Creation d'une nouvelle branche sous GithubDesktop](../assets/ghd-new-branch-button.png)

Bravo !! Vous venez de créer une *branche locale*. Etant locale elle n'apparaitra donc pas sur GitHub (elle est lier au *dépôt locale*). 
Pour pallier a ce problème vous pouvez donc simplement cliquez sur le bouton `Publiez branche` et celle si sera automatiquement mise en ligne.

![Publication d'une branch source GithubDesktop](../assets/ghd-publish-branch-button.png)

## Créer une branche grâce à Github

Connectez-vous à [github](https://github.com/login) puis sélectionné le dépôt d'intérêt. Cette technique permettra de créer une branche directement à *l'origin* (à l'inverse de locale). Appuyez sur le bouton pour selectionner votre branch et entrez dans la zone de texte le nom de votre nouvelle branche. Appuyez sur entrer une fois finit, et voilà !

![Creation d'une nouvelle branche sous GitHub](../assets/gh-create-branch.png)

<div class="note indent">
  <header>Note</header>
  <p>
    Grâce à cette technique la branche et directement créer à <i>l'origin</i>. Néanmoins elle n'apparaitra immédiatement localement. En effet pour celà il faut mettre à jour le dépot soit en appuyant sur le bouton <b>Fetch Origin</b>, sur <i>GitHub Desktop</i> soit via la commande <code>git fetch</code>
  </p>
</div>

## Créer une branche grâce au Terminal

Pour créer une branche *en locale* simplement entrez la commande suivante

```sh
git branch <nom-de-votre-branche>
```

<div class="note indent">
  <header>Note</header>
  <p>
    Le nom de votre branche ne doit pas contenir d'espace ! Utilisez des - en lieux et places. Par exemple au lieux de nommez votre branche <code>Hot Fix features</code> nommez-là <code>hot-fix-features</code>
  </p>
</div>



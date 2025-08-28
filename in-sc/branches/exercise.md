---
layout: default
title: Exercice récapitulatif
parent: "Partie 4 : Branches"
nav_order: 3
section: IN-SC
permalink: in-sc/branches/exercise
---

# Exercice récapitulatif
{: .no_toc }

Dans cet exercice, tu vas exercer tout ce que tu as vu sur les branches.

<hr>
## Table des matières
{: .no_toc.text-delta }
1. TOC
{:toc}
<hr>

## Préparatifs
Pour cet exercice, tu vas devoir télécharger un dépôt que nous avons préparé. Il contient déjà des commits et des branches.

<span class="fs-5">
  <a class="btn btn-green" href="/assets/guide-bouffe.zip" download>
    ↓ Télécharger <small>(.zip, 87 ko)</small>
  </a>
</span>

Une fois l’archive Zip téléchargée, décompresse-la.

<div class="warning">
  <header>Bonnes pratiques</header>
  <p>
    En général, ce n’est pas une bonne idée de télécharger un dépôt via une archive Zip ! Les fichiers cachés créés par Git ne sont pas conçus pour être partagés. Ici, nous te faisons télécharger le dossier pour simuler ce que tu aurais pu faire avec tes connaissances actuelles. À la place, il vaut mieux le <a href="../collaboration/remote">cloner</a>, comme nous le verrons dans la partie suivante.
  </p>
</div>

### Ajouter le dépôt à GitHub Desktop
Maintenant que tu as le dossier `guide-bouffe`, nous allons l’ajouter dans GitHub Desktop.

Sélectionne **Current Repository** en haut à gauche pour ouvrir le **sélecteur de dépôt**. Depuis cet encadré, tu peux basculer rapidement entre tes différents projets.

![“Add Existing Repository” dans le sélectionneur de dépôt](/assets/add-repo.png)

Clique alors sur **Add** > **Add Existing Repository…**. Sélectionne l’emplacement du dossier `guide-bouffe` que tu as téléchargé, puis confirme en cliquant sur **Add Repository**.

<div class="check">
  <header>Vérification</header>
  <p>Une fois que tu as bien ajouté le dépôt, tu devrais voir en haut à gauche <em>Current Repository: guide-bouffe</em>.</p>
</div>

### Ouvrir le dépôt depuis IntelliJ IDEA
Nous allons faire de même dans IntelliJ IDEA afin de pouvoir modifier les fichiers.

* Sélectionne le menu *Open*. Tu peux le trouver comme ceci :
  * Si tu viens d’ouvrir IntelliJ IDEA et que tu es sur l’**écran de démarrage**, clique sur le bouton **Open** qu’il contient.
  * Si un projet est déjà ouvert, rends-toi dans le menu **File** > **Open…**.
* Sélectionne le dossier `guide-bouffe` puis confirme.
* IntelliJ IDEA te demande si tu veux ouvrir le projet dans une nouvelle fenêtre ou remplacer la fenêtre du projet actuel. Choisis ce que tu préfères !

<div class="check">
  <header>Vérification</header>
  <p>Dans la <a href="../intellij-idea/ui#palettes-doutils">vue <em>Project</em></a>, tu dois normalement apercevoir (entre autres) le fichier <code>courses.txt</code>.</p>
</div>

## Déroulement
Le dépôt que tu as téléchargé est un recueil de conseils pour manger à Lausanne. Des ajouts de contenu ont été effectués sur d’autres branches. Nous allons les rapatrier sur la branche principale.

<div class="note">
  <header>Note</header>
  <p>Le contenu du dépôt est extrait d’un super document de conseils, que tu peux lire en entier <a href="https://drive.google.com/file/d/1CalWP-mD3B91QcW1-NZHBb2zySgkc_h1/view" target="_blank"><strong>sur le drive de Students 4 Students</strong></a> !</p>
</div>

### Changer de branche <small title="Difficulté : simple">★☆☆</small>
Actuellement, tu te situes sur la branche *main*. Rends-toi sur la branche `partie-recettes`.

<div class="check">
  <header>Vérification</header>
  <p>Dans IntelliJ IDEA, vérifie que tu as bien un dossier <code>recettes</code> qui comprend trois éléments.</p>
</div>

### Fusion sans conflits <small title="Difficulté : simple">★☆☆</small>
On aimerait intégrer les recettes à la branche principale. Fais-le en fusionnant la branche `partie-recettes` dans la branche `main`[^1].

[^1]: GitHub Desktop affichera qu’il y a des conflits dans ce merge, alors qu’il n’y en a pas. C’est un <a href="https://github.com/desktop/desktop/issues/8049" target="_blank">bug connu</a>, tu peux ignorer l’avertissement qui s’affiche.

<div class="check">
  <header>Vérification</header>
  <p>Vérifie dans GitHub Desktop que tu te trouves bien sur la branche <code>main</code>. Dans l’historique des commits, le dernier commit doit être “<em>Merge branch 'partie-recettes' into main</em>”.</p>
</div>

### Fusion avec conflits <small title="Difficulté : moyen">★★☆</small>
La branche `ajout-denner` ajoute une nouvelle entrée à la liste des supermarchés. Or, un conflit se produit car d’autres magasins ont été ajoutés au même endroit sur la branche principale depuis la création de la branche.

Fusionne la branche `ajout-denner` dans la branche `main` en réglant les conflits. Les deux paragraphes ajoutés doivent se trouver dans le résultat final. La phrase introductrice a été modifiée deux fois : à toi de la réécrire pour que toutes les informations ajoutées s’y trouvent.

<div class="check">
  <header>Vérification</header>
  <p>Vérifie dans GitHub Desktop que tu te trouves bien sur la branche <code>main</code> et qu’il n’y a aucun changement en attente de commit. Ouvre le fichier <code>courses.txt</code> depuis IntelliJ IDEA et vérifie que tout le contenu ajouté s’y trouve.</p>
</div>

## Notes de bas de page

---
layout: default
title: Initialiser un nouveau dépôt
parent: "Partie 2 : Introduction à Git"
nav_order: 1
permalink: /git-intro/init
---

# Initialiser un nouveau dépôt
Nous allons commencer par créer un nouveau **dépôt** (ou ***repository*** en anglais). Un dépôt est un dossier dans lequel Git est actif. Nous allons créer un nouveau dépôt à partir du projet que tu as créé lors de la partie précédente, mais tu peux aussi le faire à partir d’un autre projet si tu le préfères.

## Comment faire

Ouvre GitHub Desktop, puis va dans le menu *File*, et sélectionne *New Repository*.

Remplis le formulaire *“Create a New Repository”* comme ceci :
* ***Name*** : le nom du dossier du projet que tu as créé (par exemple *hello-world*).
* ***Description*** : tu peux laisser ce champ vide.
* ***Local Path*** : sélectionne le dossier **au-dessus** de celui qui contient ton projet.

<div class="warning indent">
  <header>Avertissement</header>
  <p>
    Il faut bien que tu sélectionnes le dossier <strong>parent</strong> de celui de ton projet. Sinon, GitHub Desktop va créer un nouveau dossier à l’intérieur de ton projet qui porte le même nom, et les autres fichiers de ton projet ne seront donc pas dans le dépôt.
  </p>
  <p>
    Par exemple, si tu as créé ton projet dans le dossier <em>Documents</em>, sélectionne le dossier <em>Documents</em> dans <em>Local Path</em>.
  </p>
</div>

* ***Initialize this repository with a README*** : tu peux laisser décoché.

<div class="tip indent">
  <header>Bon à savoir</header>
  <p>
    Souvent, les projets de programmation contiennent un fichier nommé README (en français : <em>Lisez-moi</em>) qui contiennent une brève présentation du projet ainsi que d’autres informations utiles.
  </p>
</div>

* ***Git Ignore*** : Tu peux demander à Git d’ignorer certains fichiers pour que leurs modifications ne soient pas tracées. C’est notamment utile pour les fichiers temporaires, les fichiers de configuration de ton éditeur, et les fichiers qui contiendraient des informations sensibles (comme des mots de passe). Ici, GitHub Desktop te propose plusieurs réglages par défaut, sélectionne celui nommé **Java**.

<div class="tip indent">
  <header>Bon à savoir</header>
  <p>
    Ces réglages seront stocké dans un fichier dans ton projet nommé <code>.gitignore</code>, que tu peux toujours modifier par la suite. Si nécessaire, tu peux trouver plus d’informations sur Internet à propos du fonctionnement de ces fichiers.
  </p>
</div>

* ***License*** : tu peux choisir de publier ton projet sous une licence libre, qui fixe les conditions sous lesquelles quiconque peut utiliser ton projet. Ici, tu peux laisser vide (*None*).

<div class="note indent">
  <header>Note</header>
  <p>
    Si tu as envie de plus d’informations sur les différentes licences, le site <a href="https://choosealicence.com" target="_blank">choosealicence.com</a> édité par GitHub offre un bon résumé.
  </p>
</div>

<figure>
  <img src="{{ '/assets/init.png' | relative_url }}" alt="La fenêtre “Create a New Repository”">
</figure>

Une fois que tu as tout rempli, clique sur ***Create Repository***. Et voilà, ton dépôt est créé !

---
layout: default
title: Visualiser l’historique
parent: "Partie 3 : Introduction à Git"
nav_order: 3
section: IN-SC
permalink: in-sc/git-intro/history
---

# Visualiser l’historique
Quelque chose de très pratique avec Git est la possibilité de voir toutes les modifications qui ont été faites sur un projet par le passé.

GitHub Desktop te permet de visualiser cela dans un écran dédié. Pour l’ouvrir, clique sur **History** en haut à gauche.

![La vue History de GitHub Desktop](/assets/history.png)

À gauche se situe la liste des derniers commits. Lorsque tu en sélectionnes un, les modifications effectuées lors de ce commit s’affichent sur la droite de la fenêtre.

Lorsque tu sélectionnes un fichier modifié contenant du code les lignes ajoutées s’affichent en vert, et celles qui ont été supprimées sont en rouge. Et lorsque tu sélectionnes une image, GitHub Desktop affiche une vue permettant de voir visuellement les différences.

![Affichage des modifications effectuées sur une image](/assets/diff-image.png)

## Trouver l’origine d’une modification
Git offre une autre fonctionnalité intéressante appelée **blame**. Elle permet de savoir dans quel commit une ligne de code de ton projet a été écrite. Nous allons utiliser la fonctionnalité intégrée dans IntelliJ IDEA pour le faire.

Ouvre un fichier de ton choix dans IntelliJ IDEA. Dans la [recherche globale](../intellij-idea/ui#recherche-globale), écris `blame` puis active **Git \| Current File: Annotate with Git Blame**.

Dans la colonne de gauche, la date et l’auteur/autrice du commit sont indiqués. Tu peux cliquer dessus pour voir les autres détails (message, description, fichiers modifiés…).

![Affichage d’un “blame” dans IntelliJ IDEA](/assets/blame.png)

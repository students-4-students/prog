---
layout: default
title: Créer votre premier projet
parent: "Partie 2 : IntelliJ IDEA"
nav_order: 1
permalink: /intellij-idea/first-project
---

# Créer votre premier projet

Commençons par ouvrir IntelliJ et créer le premier projet de programmation Java que tu réaliseras cette année. Le but de ce dernier sera simple : afficher sur la console une simple phrase "Hello world". Il va cependant être nécessaire de préparer un peu le terrain avant de passer au code.

## Initialiser le projet et installation du JDK
* Première étape : créer un nouveau projet (Si l'interface est en anglais, *New Project*)

![Fenêtre de démarrage IntelliJ](./assets/home-intellij.jpg)

Pour pouvoir développer des applications en Java, tu vas devoir installer un **JDK** (Java Development Kit). Il existent plusieurs versions et plusieurs éditeurs de JDK, mais pour ton utilisation nous te recommandons d'installer **OpenJDK 11**.

<div class="Note">
  <header>Le Java Development Kit ?</header>
  <p>
    Cela va peut-être te paraître encore un peu obscure, mais tout vas bien se passer ne panique pas. Le JDK est un ensemble d'outils et bibliothèques de base de Java qui permettront à ton ordinatinateur de compiler et d'exécuter ton projet et d'utiliser des fonctionnalités grâce aux "bibliothèques" Java.
  </p>
</div>

* Pour installer le OpenJDK 11, sélectionner *Download JDK* dans le menu déroulant intitulé *Project SDK*.

![Emplacement sélection JDK](./assets/jdk-prj.png)

* Une fenêtre d'options va apparaître. Sélectionner la **Version 11**  et **AdoptOpenJDK** comme *Vendor*. Inutile de modifier le dossier d'installation. Installer à présent le JDK en cliquant sur *Download*

## Dernières options

* Sélectionner deux fois *Next* pour arriver à la partie configuration finale du projet. Nous intitulerons le projet **"Hello-World"**. Tu peux décider de créer le projet dans le dossier que tu souhaites avec *Project location*.

![Finalisation de la création du projet](./assets/project-setup.jpg)

Et voilà ! Une fois que tu auras appuyé sur *Finish*, ton projet sera créer.

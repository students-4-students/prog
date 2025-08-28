---
layout: default
title: Exécuter un programme
parent: "Partie 2 : IntelliJ IDEA"
nav_order: 3
section: IN-SC
permalink: in-sc/intellij-idea/run
---

# Exécuter un programme
{: .no_toc }

Maintenant que le projet a été configuré et que tu as eu un aperçu des fonctionnalités d'IntelliJ IDEA, il est temps de réaliser ton premier programme en Java.

<hr>
## Table des matières
{: .no_toc.text-delta }
1. TOC
{:toc}
<hr>

## Créer un fichier sur IntelliJ IDEA
Dans la [vue *Project*](ui#palettes-doutils), tu devrais voir un dossier nommé `src`. Par convention, ce dossier contient tout le code que tu écriras : c'est le dossier source. Pour ce qui est des autres fichiers comme les images ou sons, il est d’usage de les mettre dans un dossier ressources à part (souvent nommé `resources`).

<div class="note">
  <header>Dossiers source, ressources, etc.</header>
  <p>Le dossier `src` devrait s’afficher avec une icône bleue, car IntelliJ IDEA l’a automatiquement reconnu comme dossier source. Si tu aimerais changer la structure des dossiers (par exemple pour créer un dossier ressources), tu auras besoin de refaire manuellement les associations.</p>
  <p>Pour le faire, fais un clic droit sur le dossier, puis sélectionne <em>Sources Root</em> (pour le dossier source) ou <em>Resources Root</em> (pour le dossier ressources) sous <em>Mark Directory as</em>.</p>
  <img src="/assets/mark-directory-as.png" alt="Localisation du menu “Mark Directory as”">
  <p>Vérifier que les associations sont bien faites peut t’être utile si tu rencontres un problème avec un projet, par exemple lorsque tu importes un projet créé avec un autre IDE.</p>
</div>

Nous allons ajouter un fichier au dossier `src`. Pour cela, fais un clic droit sur le dossier `src` et sélectionne *New* > *Java Class*. Donne-lui le nom `HelloWorld`.

![Création du fichier](/assets/file-created.png)

IntelliJ IDEA génère automatiquement l'entête de la classe comme ci-dessus. Il ne reste plus qu'à écrire notre code. À ce stade, tu n’as pas besoin de savoir ce qu’est une classe. Ne t’inquiète pas, ce sera expliqué en classe ce semestre&nbsp;!

## Écrire le programme
Maintenant, écrivons le contenu de notre programme. Si tu ne comprends pas bien comment tout cela marche, ce n’est pas grave, les détails te seront expliqués ce semestre.

Change le contenu du fichier `HelloWorld.java` pour qu’il contienne :

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.printf("Hello world!");
    }
}
```

<div class="tip">
  <header>Astuce</header>
  <p>Pour écrire ce code plus rapidement, tu peux utiliser les raccourcis suivants :</p>
  <ul>
    <li>
      <code>psvm</code> pour écrire <code>public static void main(String[] args) { }</code>,
    </li>
    <li>
      et <code>sout</code> pour écrire <code>System.out.println();</code>.
    </li>
  </ul>
  <p>Ces raccourcis s’affichent dans l’<strong>autocomplétion</strong>, qui est une liste de suggestions qu’IntelliJ IDEA te propose lorsque tu es en train d’écrire. Tu peux choisir une option avec les touches fléchées, et valider ton choix avec la touche <em>Enter</em>.</p>
  <video autoplay loop muted playsinline src="/assets/autocomplete.mp4"></video>
  <p>Tu peux trouver d’autres raccourcis, et même configurer les tiens, dans la section <em>Live Templates</em> des réglages (que tu peux atteindre en utilisant la <a href="ui#recherche-globale">recherche globale</a>).</p>
</diV>

## Exécuter un programme
Ton programme est prêt à être exécuté, testons le dès à présent.

Si tu regardes bien dans le coin supérieur droit, tu peux trouver une sorte de bouton « play » grisé. Tu pourras l’utiliser dans le futur pour lancer ton programme, mais il est pour le moment inopérant car aucune exécution n’a été configurée.

Pour configurer l’exécution de ton programme, clique sur l'un des deux boutons « play » situés juste à la gauche de ton code, puis *Run 'HelloWorld.main()'*. Cela va directement exécuter la fonction `main` (tu verras en cours ce qu’est exactement une fonction).

![Résultat d'exécution du programme](/assets/hello-world.png)

Tu devrais normalement obtenir le résultat ci-dessus. Bravo, tu as conçu ton premier programme en Java !

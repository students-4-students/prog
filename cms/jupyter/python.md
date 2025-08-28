---
layout: default
title: Découvrir Jupyter
parent: "Partie 2 : Jupyter Notebook"
nav_order: 2
section: CMS
permalink: cms/jupyter/python
---

# Découvrir Jupyter

## Qu'est-ce qu'une cellule dans Jupyter ?

Dans Jupyter Notebook, un **notebook** est composé de plusieurs **cellules**. Chaque cellule peut contenir du **code**, des **commentaires** ou des **visualisations**. Il existe principalement deux types de cellules : les cellules de code et les cellules de texte (ou cellules Markdown).

### Types de cellules

1. **Cellule de code** : C’est ici que tu écris ton programme Python.
2. **Cellule Markdown** : Tu peux y ajouter des explications ou des titres. C’est une manière d’organiser ton notebook.

## Comment ajouter une cellule ?

Pour ajouter une nouvelle cellule, il te suffit de cliquer sur le bouton **+** dans la barre d'outils de Jupyter.

![Ajouter une cellule](/assets/jupyter-add-cell.png)

Tu peux ensuite choisir si tu veux une cellule de code ou une cellule Markdown en utilisant les options dans le menu déroulant en haut à gauche (par défaut, les nouvelles cellules sont des cellules de code).

## Comment exécuter une cellule ?

Une fois que tu as écrit du code dans une cellule, tu peux l'exécuter pour voir les résultats. Pour ce faire, il suffit de cliquer sur la cellule que tu veux exécuter, puis :

1. Appuie sur **Shift + Enter** pour exécuter la cellule et passer à la suivante.
2. Ou bien, clique sur le bouton **Run** dans la barre d'outils pour exécuter la cellule.

### Exemple de code dans une cellule :

Écris simplement ton code Python dans la cellule et exécute-le. Par exemple, pour afficher un message, tu peux utiliser :

```python
print("Bonjour, Jupyter !")
```

Une fois exécuté, tu verras la sortie directement sous la cellule.

![Exécution d'une cellule de code](/assets/jupyter-run-cell.png)

### Sortie de la cellule

Lorsque tu exécutes une cellule contenant du code, la sortie (résultats, erreurs ou affichage) apparaît juste en dessous de la cellule. C'est là que tu verras par exemple le résultat d'un calcul, un graphique ou un message comme dans l'exemple ci-dessus.

## Comment modifier et réexécuter une cellule ?

Si tu veux modifier une cellule après l'avoir exécutée, clique simplement sur la cellule, fais tes modifications, puis exécute-la à nouveau. Par exemple, si tu veux changer le message affiché dans le code précédent :

```python
print("Ceci est une modification du message.")
```

Il te suffit d'appuyer à nouveau sur **Shift + Enter** ou de cliquer sur **Run** pour voir la nouvelle sortie.

<div class="note">
  <header>Résumé</header>
  <ul>
    <li><strong>Ajouter une cellule</strong> : Clique sur <strong>+</strong> pour ajouter une nouvelle cellule.</li>
    <li><strong>Exécuter une cellule</strong> : Appuie sur <strong>Shift + Enter</strong> ou clique sur <strong>Run</strong> pour exécuter ton code.</li>
    <li><strong>Cellules de texte</strong> : Utilise des cellules Markdown pour ajouter des explications et organiser ton notebook.</li>
  </ul>
</div>

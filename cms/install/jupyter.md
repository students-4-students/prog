---
layout: default
title: Installer Jupyter
parent: "Partie 1 : Installations"
nav_order: 2
section: CMS
permalink: cms/install/jupyter
---

# Installation
{: .no_toc }

Après avoir installé Python 3, nous allons maintenant installer Jupyter Notebook. 

### Vérification de pip

Pip est le gestionnaire de paquets de Python, essentiel pour installer et gérer les bibliothèques. Avant de commencer l'installation de Jupyter, il est important de vérifier si pip est déjà installé sur ton système. Pour cela, ouvre un terminal et tape la commande suivante :

```bash
python3 -m pip --version
```

Si cette commande ne génère aucune erreur et affiche un numéro de version, cela signifie que pip est installé. Dans certains cas, selon ton système, il faudra peut-être utiliser :

```bash
python -m pip --version
```

### Installation de Jupyter Notebook

Une fois que pip est configuré, tu peux installer Jupyter Notebook. Voici les étapes à suivre :

1. Ouvre un terminal et installe Jupyter en utilisant pip :

   ```bash
   python3 -m pip install notebook
   ```
Sur certains systèmes, remplace python3 par python selon ta configuration.


2. Une fois l'installation terminée, dirige-toi vers le dossier où tu souhaites créer ou ouvrir un notebook, puis lance Jupyter en tapant :

   ```bash
   jupyter notebook
   ```

   Cette commande ouvrira automatiquement Jupyter dans ton navigateur par défaut. La racine de Jupyter sera le dossier dans lequel tu as exécuté la commande.

3. Pour fermer Jupyter Notebook, il te suffit de revenir dans le terminal où il est lancé et d'appuyer sur `Ctrl + C`.

### Vérification de l'installation

Après avoir installé Jupyter, tu peux vérifier que l'installation a réussi en exécutant la commande suivante :

```bash
jupyter --version
```

Cela te donnera la version actuellement installée sur ton système. Si tu rencontres une erreur, cela peut indiquer que l’installation n’a pas réussi.




---
layout: default
title: Installer Python
parent: "Partie 1 : Installations"
nav_order: 1
section: CMS
permalink: cms/install/python
---

# Installer Python
{: .no_toc }

Dans cette section, nous allons t'expliquer comment installer Python, l'un des langages les plus utilisés pour la programmation scientifique et algorithmique.

<div class="tip indent">
  <header>Astuce</header>
  <p> Assure-toi de cocher la case <strong>Add Python to PATH </strong> avant de cliquer sur Install Now. Cela te permettra d'utiliser Python facilement depuis n'importe quel terminal.</p>
</div>


### Windows

Rends-toi sur le site officiel de Python à l’adresse [python.org/downloads](https://www.python.org/downloads/), et clique sur **Download Python** pour télécharger le fichier d'installation adapté à ta version de Windows. Une fois téléchargé, double-clique sur le fichier *.exe* pour commencer l’installation. Une fenêtre similaire à l'image ci-dessous devrait apparaître:


![Écran de téléchargement Python Windows](/assets/python-download-windows.png)



### Mac

Rends-toi sur le site officiel de Python à l’adresse [python.org/downloads](https://www.python.org/downloads/), et clique sur **Download Python** pour macOS. Une fois téléchargé, ouvre le fichier *.pkg* pour démarrer l’installation et suis les instructions à l'écran.



### Linux

Sur Linux, tu peux installer Python directement via ton gestionnaire de paquets. Ouvre un terminal et tape la commande suivante :

```bash
sudo apt update
sudo apt install python3
```

Cela installera la dernière version stable de Python.

## Vérification de l'installation

Une fois Python installé, tu peux vérifier que tout s'est bien passé en ouvrant un terminal et en tapant la commande suivante :

```bash
python3 --version
```

ou sur certains systèmes:

```bash
python --version
```

Tu devrais alors voir une réponse du type  :

```
Python 3.13.6
```

Si la version de Python apparaît sans erreur, cela signifie que l’installation a été effectuée avec succès.





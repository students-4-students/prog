---
layout: default
title: "Partie 4 : Branches"
nav_order: 4
has_children: true
permalink: /branches/
---

# Utiliser les branches
Dans cette partie, tu vas découvrir une fonctionnalité très pratique de Git : les **branches**.

Les branches sont un mécanisme qui permet de séparer un projet en **plusieurs versions distinctes** qui peuvent évoluer chacune séparément. À tout moment, tu peux décider de **fusionner** deux branches, ce qui consiste à effectuer sur une branche les changements faits sur une autre.

## Un exemple
Pour l’instant, tout cela peut te sembler très abstrait, alors voici un exemple de comment tu peux utiliser les branches lorsque tu développes un logiciel.

Lorsque tu as [initialisé le dépôt](../git-intro/init), tu t’es retrouvé sur sa **branche principale** qui est nommée dans la plupart des projets *main* ou *master*[^1]. Cette branche contiendra la version la plus stable de ton logiciel, où toutes les fonctionnalités sont achevées (donc la version que tu distribueras aux personnes qui utilisent ton programme).

Maintenant, disons que tu veux développer une nouvelle fonctionnalité. Tu crées donc une **nouvelle branche** portant le nom de ta fonctionnalité, disons *ma-super-fonctionnalité*. Selon son ampleur, il faudra peut-être plusieurs commits pour la finaliser, que tu effectueras tous sur cette branche.

Pendant ce temps, les autres branches pourront évoluer librement chacune de leur côté (ce qui sera très pratique si tu travailles à plusieurs !). Une fois ton travail achevé, tu pourras fusionner la branche *ma-super-fonctionnalité* dans la branche principale, pour que toutes les modifications que tu as faites s’y retrouvent. Cela fonctionne même si d’autres modifications ont été faites entre temps sur la branche principale !

![Fonctionnement des branches sous Git](../assets/branches.svg)

## Un autre exemple
Imagine que tu dois travailler sur une nouvelle fonctionnalité d’une application que nous appellerons *Feature 05*, tu crées pour ce faire une branche nommée `feature-05` (oui nous autres programmeurs, débordons d'imagination). Soudain, ton coéquipier te signale que la fonctionnalité *Feature 03* ne fonctionne pas.

Grâce à *Git*, tu n'es pas obligée d'écrire le correctif directement sur la branche en cours (`feature-05`). Tu peux tout d'abord changer de branche et te mettre sur la `master` puis créer une nouvelle branche `hotfix-feature-03` depuis la `master` (branche qui n'aura pas encore les modifications apportées à `feature-05`). Tu résous ensuite le bug sur la branche `hotfix-feature-03` sans te préoccuper de *Feature 05* (étape très sympathique). Et une fois que les modifications sont faite tu fusionne la branche `hotfix-feature-03` à la `master`, et voilà !!

<div class="note indent">
  <header>Note</header>
  <p>
    Si tu veux tes correctifs de bug, dans la branche <code>feature-05</code> il te faut ensuite fusionner la <code>master</code> à cette branche, via un <code>git merge</code>
  </p>
</div>


<hr>

[^1]: Le nom utilisé par défaut pour la branche principal a longtemps été *master*. Ce nom est actuellement en train d’être remplacé par *main* pour éviter la terminologie liée à l’esclavagisme (*maître*/*esclave*) dont il était issu. Les nouveaux dépôts créés sur GitHub ou avec GitHub Desktop <a href="https://github.com/github/renaming" target="_blank">utilisent désormais *main*</a>, et un changement similaire est en train d’être effectué <a href="https://lore.kernel.org/git/xmqqa6vf437i.fsf@gitster.c.googlers.com/T/#t" target="_blank">dans Git lui-même</a>.


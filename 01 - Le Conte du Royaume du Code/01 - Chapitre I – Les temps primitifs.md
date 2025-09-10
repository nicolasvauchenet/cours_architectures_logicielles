# Chapitre I – Les temps primitifs (années 40–60)

![chapitre I.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-I.png)

À l’aube des temps numériques, seuls quelques initiés comprenaient la langue des machines : une suite de `0` et de `1`,
sans poésie apparente mais porteuse d’une puissance inouïe. On ne “parlait” pas encore d’architectures logicielles,
mais de calculs, de guerre froide, et d’équipes de savants enfermés dans des laboratoires où cliquetaient des relais et
chauffaient des lampes à vide.

Les premiers héros furent **Alan Turing**, qui en 1936 imagina une *machine universelle* capable de simuler tout calcul
possible, et **John von Neumann**, qui proposa en 1945 un modèle d’ordinateur où les instructions et les données
cohabitent en mémoire. Ces concepts théoriques, semblables à des plans de cathédrales dessinés sur parchemin,
allaient devenir la charpente invisible de toutes les machines futures.

---

## Des cabanes de bits et de registres

Les premiers programmes étaient écrits en **code machine** : une suite de nombres binaires directement interprétés par
les circuits. Cela revenait à construire une maison en plantant chaque clou un par un, sans plan, sans outils, et en
retenant de mémoire l’emplacement exact de chaque planche.

Puis vint l’**assembleur**, une étape au-dessus : on pouvait enfin utiliser des **mnémoniques** comme `MOV`, `ADD` ou
`JMP` au lieu de simples zéros et uns. Les programmeurs parlaient d’être “proches du métal” : chaque instruction était
une étincelle électrique dans les entrailles de la machine. Mais ce confort restait relatif : changer une boucle
pouvait signifier déplacer des dizaines d’adresses mémoire, comme si l’on devait redessiner toute une charpente pour
déplacer une simple fenêtre.

> « Programmer en assembleur, c’est comme sculpter avec un marteau-piqueur : possible, mais épuisant. »

---

## Les pionniers et leurs monstres mécaniques

L’histoire des années 40–60 est une galerie de machines légendaires :

- **ENIAC (1945)** : premier grand calculateur électronique, 30 tonnes de matériel, 18 000 tubes à vide, et une
  programmation réalisée en reliant des câbles.
- **EDSAC (1949, Cambridge)** : première machine à implémenter l’architecture de von Neumann.
- **IBM 701 (1952)** : surnommé la “Defense Calculator”, conçu au cœur de la guerre froide pour des simulations
  nucléaires.
- **IBM System/360 (1964)** : révolution car il introduit une **famille compatible de machines**, marquant la première
  pierre d’une stratégie logicielle cohérente.

Chaque machine était un monstre coûteux, installé dans des salles climatisées, mais aussi une **boîte noire fragile** :
le programme n’existait que tant que la mémoire était alimentée. Couper l’électricité, c’était effacer le savoir.

---

## Les limites du bricolage

Écrire du code dans ces conditions, c’était bâtir des huttes instables sur un sol mouvant. Le moindre changement
exigeait
souvent de tout reconstruire. Les registres et adresses mémoire dictaient leur loi, et la logique métier – quand il y en
avait une – était noyée sous une avalanche de détails techniques.

Un simple bug pouvait mettre des jours à être identifié. Les programmeurs devenaient des archéologues dans leurs
propres ruines, fouillant les entrailles du code pour trouver l’instruction fautive.

Cette époque fut un âge héroïque, mais aussi un **âge de souffrance**. De nombreux témoignages de programmeurs de
l’époque décrivent des nuits blanches passées à corriger des erreurs “invisibles” pour l’œil humain, mais fatales pour
la machine.

> « J’avais trouvé l’erreur : un seul `0` à la place d’un `1`. Deux jours perdus. »  
> — Témoignage d’un ingénieur du MIT, 1957

---

## L’appel de l’abstraction

À mesure que les besoins croissaient – calculs militaires, prévisions météo, gestion de bases de données rudimentaires –
il devenait clair qu’il fallait échapper à cette prison binaire. Les bâtisseurs pressentaient déjà qu’il fallait lever
les yeux du métal et inventer des **langages de plus haut niveau**.

Les premiers jalons furent posés : **Fortran** (1957, IBM) pour les scientifiques, **LISP** (1958, John McCarthy) pour
l’intelligence artificielle naissante, **COBOL** (1959, commission dirigée par Grace Hopper) pour l’administration et
la gestion. Ces langages allaient donner aux programmeurs de véritables briques réutilisables et un vocabulaire plus
riche, ouvrant la voie aux “architectures” logicielles à venir.

---

## Métaphore finale

On peut voir cette époque comme l’âge où l’humanité, encore vêtue de peaux de bêtes, dressa ses premiers abris contre le
vent. Ces cabanes de bois – les programmes en assembleur – n’étaient pas encore des châteaux ni des villes, mais elles
montraient déjà une intention : celle de bâtir plus grand, plus solide, et plus durable.

> La puissance brute existe, mais la maintenabilité manque.  
> C’est cette tension qui allait guider toute l’histoire de l’architecture logicielle.

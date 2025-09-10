# Chapitre II – Le Bâtisseur C (années 70)

![chapitre II.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-II.png)

Les années 70 furent marquées par une effervescence intellectuelle. Dans un coin discret des laboratoires **Bell Labs**,
une poignée de chercheurs façonna un langage qui allait devenir la charpente invisible de l’informatique moderne.  
L’artisan en chef s’appelait **Dennis Ritchie**. Son outil : le **langage C**.

---

## La forge de Bell Labs

En 1969, Ken Thompson avait déjà conçu un premier système d’exploitation nommé **UNIX**. Il l’avait écrit en **B**, un
langage de programmation minimaliste dérivé de **BCPL**. Mais ce langage, frêle esquisse, manquait de muscles. C’est là
que Ritchie intervint : il forgea **C**, une évolution qui combinait puissance et expressivité.

En **1972**, UNIX fut réécrit en C. C’était une révolution : jusque-là, les systèmes d’exploitation étaient écrits en
assembleur, et donc intimement liés au matériel sur lequel ils tournaient. Réécrire un OS dans un langage de haut niveau
ouvrait la voie à une idée audacieuse : **la portabilité**. UNIX pouvait désormais voyager d’une machine à l’autre,
comme une caravane traversant le désert, transportant son savoir dans ses bagages.

---

## Les compagnons de route

- **Ken Thompson**, déjà père d’UNIX, adopta immédiatement C pour développer ses outils et solidifier l’édifice.
- **Brian Kernighan**, écrivain technique talentueux, comprit qu’un langage sans livre est comme une cathédrale sans
  vitraux : invisible aux yeux des profanes. Avec Ritchie, il publia en **1978** *The C Programming Language*, connu
  simplement comme *K&R*. Ce livre, sobre et clair, devint la Bible des programmeurs.

> « C est à la fois puissant et dangereux : il vous donne le contrôle total, mais il exige que vous sachiez ce que vous
> faites. »  
> — Brian Kernighan, entretien (1981)

---

## La révolution de la portabilité

L’impact de C fut immédiat. Des projets entiers basculèrent vers ce langage :

- Les systèmes d’exploitation, avec UNIX en tête, mais aussi plus tard **Windows NT** (dont une grande partie du noyau
  fut écrite en C).
- Les compilateurs : écrire un compilateur en C permettait de créer une chaîne capable de s’auto-reproduire sur de
  nouvelles machines.
- Les bases de données : **Oracle** (1977) et **Ingres**, puis **PostgreSQL** (dès 1986, issu du projet Postgres de
  Michael Stonebraker) virent le jour grâce à C.

C’est comme si le langage avait offert aux bâtisseurs une **pierre universelle**, pouvant être taillée et ajustée à
n’importe quel chantier.

---

## La puissance et ses périls

La force de C résidait dans son efficacité : les programmes étaient rapides, compacts, et offraient un contrôle précis
sur la mémoire. On pouvait manipuler des **pointeurs** pour accéder directement à n’importe quelle zone mémoire, comme
un architecte pouvant toucher chaque pierre du château.

Mais ce don était une arme à double tranchant. La moindre erreur – un pointeur mal initialisé, une zone mémoire mal
libérée – pouvait provoquer l’effondrement complet du programme. Là où les langages plus abstraits mettaient des
garde-fous, C confiait au développeur une liberté totale. La robustesse ne venait pas du langage, mais de la *
*discipline
et de la rigueur** de ceux qui l’utilisaient.

> « C combine la puissance de l’assembleur avec la commodité… de l’assembleur. »  
> — dicton humoristique de l’époque

---

## Anecdotes et héritage

On raconte qu’au début des années 70, dans les couloirs des Bell Labs, un jeune programmeur demanda pourquoi Ritchie
avait appelé son langage “C”. La réponse fut simple : parce qu’il venait après “B”. Une explication modeste, presque
ironique, pour un outil qui allait pourtant fonder des empires numériques.

Aujourd’hui encore, derrière nos navigateurs modernes et nos applications mobiles, le langage C se cache comme une
fondation silencieuse. Les noyaux Linux, Windows, macOS, ainsi que des moteurs critiques comme **Git**, **MySQL** ou
**Python** lui doivent leur existence.

---

## Métaphore finale

Si les programmes des années 40–60 étaient des cabanes de fortune dressées dans les clairières, le langage C fut le
premier **outil de maçonnerie véritable**. Avec lui, on pouvait bâtir des châteaux solides, portables, capables de
résister au temps. Mais ces pierres taillées exigeaient des mains habiles : mal posées, elles pouvaient faire s’écrouler
tout l’édifice.

> **C donna la robustesse, mais exigea discipline et rigueur.**

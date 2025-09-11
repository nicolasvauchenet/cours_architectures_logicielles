# Chapitre I – Les Temps Primitifs (années 40–60)

![chapitre-I.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-I.png)

## Les premiers chuchotements du code

Le Royaume du Code naquit dans les ténèbres de la Seconde Guerre mondiale et de la guerre froide naissante.  
Quelques mages mathématiciens et ingénieurs, cloîtrés dans des laboratoires, maniaient un langage secret : une litanie
de `0` et de `1`.

En **1936**, Alan Turing rédigea son traité sur la *Machine universelle*.  
Un artefact purement théorique, mais capable de simuler n’importe quel calcul imaginable.  
Cette vision prophétique devint la base conceptuelle de toute informatique moderne.

En **1945**, John von Neumann proposa son *architecture*.  
Un modèle d’ordinateur où les instructions et les données
résident ensemble en mémoire.  
Ce schéma, simple mais puissant, sera adopté par presque toutes les machines à venir.  
Ces deux penseurs furent les premiers architectes spirituels du royaume.

---

## Les monstres mécaniques

Les bâtisseurs de l’époque invoquèrent des colosses de cuivre et de verre, bardés de câbles et de lampes à vide :

- **Colossus (1943, Royaume-Uni)** : utilisé par Alan Turing et ses compagnons de Bletchley Park pour décrypter les
  codes allemands (Enigma, Lorenz).
- **ENIAC (1945, États-Unis)** : premier grand calculateur électronique. 30 tonnes, 150 kW d’électricité, 18 000 tubes à
  vide. Programmé en reliant physiquement des câbles.
- **EDSAC (1949, Cambridge)** : premier ordinateur opérationnel à incarner l’architecture de von Neumann.
- **UNIVAC I (1951)** : le premier ordinateur commercial, vendu aux entreprises et administrations.
- **IBM 701 (1952)** : surnommé la *Defense Calculator*, pensé pour des calculs militaires stratégiques.
- **IBM System/360 (1964)** : révolution industrielle en proposant une famille entière de machines compatibles.

Ces monstres occupaient des salles entières, exigeaient une climatisation permanente, et tombaient souvent malades.  
Leur puissance était colossale pour l’époque, mais minuscule face au moindre smartphone moderne.

---

## Des cabanes de bits

Programmer ces créatures revenait à parler leur langue maternelle : le **code machine**, une suite d’instructions
binaires.  
Chaque `0` et `1` déclenchait un mouvement d’électrons dans les entrailles métalliques.

Cette tâche était aussi pénible que de bâtir une hutte sans plan, en plantant chaque clou un par un.  
Le moindre décalage d’adresse mémoire pouvait condamner tout un programme.

L’**assembleur** offrit une première bouffée d’air.  
Au lieu de chiffres obscurs, on écrivait des mnémoniques comme `MOV`, `ADD` ou `JMP`.  
On parlait alors d’être *proche du métal* : chaque instruction frappait directement la pierre brute de la machine.

> « Programmer en assembleur, c’est comme sculpter avec un marteau-piqueur : possible, mais épuisant. »  
> — dicton des bâtisseurs de l’époque

---

## Les héros et leurs souffrances

Les programmeurs de ces temps primitifs étaient des pionniers et des martyrs.  
Ils passaient des nuits entières à chercher des erreurs invisibles, parfois causées par un seul bit mal placé.

> « J’avais trouvé l’erreur : un seul `0` à la place d’un `1`. Deux jours perdus. »  
> — témoignage d’un ingénieur du MIT, 1957

La mémoire était instable : parfois, une simple coupure de courant effaçait toutes les données.  
Chaque bug était une bataille d’archéologie numérique, où les bâtisseurs fouillaient dans leurs propres ruines.

---

## L’appel de l’abstraction

À mesure que les besoins grandissaient (prévisions météo, gestion de données, calculs financiers), les bâtisseurs
comprirent qu’ils devaient sortir de la prison binaire.  
Il fallait inventer des langages plus proches de l’humain.

Les premières grandes innovations furent :

- **Fortran (1957, IBM)** : premier langage de haut niveau largement diffusé, pensé pour les scientifiques.
- **LISP (1958, John McCarthy)** : conçu pour manipuler des symboles et amorcer la recherche en intelligence
  artificielle.
- **COBOL (1959, Grace Hopper et son comité)** : destiné à l’administration et aux entreprises, pour écrire des
  programmes en langage “proche de l’anglais”.

Ces langages permirent enfin d’écrire du code lisible, de réutiliser des briques, et d’oser bâtir plus grand que des
huttes éphémères.

---

## Les avantages et limites de l’époque

Malgré leurs faiblesses criantes, ces machines primitives représentaient une avancée prodigieuse. Pour la première fois,
l’humanité possédait des outils capables d’accomplir en quelques secondes des calculs qui auraient demandé des semaines
de travail aux meilleurs savants. L’apparition de langages comme Fortran, LISP et COBOL offrait aussi une première
abstraction au-dessus du métal : les bâtisseurs ne parlaient plus uniquement en zéros et en uns, mais pouvaient enfin
échanger des concepts communs, un vocabulaire partagé entre équipes de chercheurs et d’ingénieurs.

**Les Forces** :

- Première abstraction au-dessus du métal.
- Machines capables de calculer en quelques secondes ce qui prenait des semaines aux humains.
- Premiers langages partagés entre équipes.

Mais cette puissance avait un prix. Les colosses de cuivre et de verre étaient fragiles : les tubes à vide claquaient
sans prévenir, la mémoire s’effaçait au moindre tremblement ou coupure d’électricité. Le coût d’une seule de ces
machines équivalait à des millions de dollars, un luxe réservé aux grandes puissances militaires, aux universités
prestigieuses ou aux multinationales naissantes. La programmation, encore ardue et obscure, restait l’apanage d’une
élite de mathématiciens et de logiciens capables de dialoguer avec ces monstres capricieux. Et surtout, aucune méthode
n’existait pour guider la construction du code : chaque bâtisseur improvisait, inventait son style, laissant derrière
lui des édifices uniques mais souvent incompréhensibles pour les générations suivantes.

**Les Faiblesses** :

- Fragilité matérielle (tubes à vide qui claquent, mémoire instable).
- Coût astronomique (des millions de dollars par machine).
- Programmation encore ardue, réservée à une élite.
- Absence de méthodes structurées : chaque bâtisseur inventait son style.

---

## Moralité

Les Temps Primitifs furent à la fois un âge de héros et un âge de souffrance.
Les bâtisseurs y posèrent les premières pierres du Royaume du Code, mais leurs édifices restaient fragiles et
instables.

> La puissance brute existe, mais sans abstractions ni méthodes, elle demeure une cabane chancelante dans la
> tempête.

Cet appel à l’abstraction allait guider toute l’histoire de l’architecture logicielle.

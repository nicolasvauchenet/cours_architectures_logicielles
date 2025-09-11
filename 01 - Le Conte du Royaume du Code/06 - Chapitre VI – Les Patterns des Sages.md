# Chapitre VI – Les Patterns des Sages (1994 et après)

![chapitre-VI.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-VI.png)

En **1994**, quatre érudits, surnommés par la suite le **Gang of Four** – **Erich Gamma**, **Richard Helm**, **Ralph
Johnson** et **John Vlissides** – publièrent un grimoire qui allait devenir un classique du Royaume du Code :  
**Design Patterns: Elements of Reusable Object-Oriented Software**.

Ce livre condensait l’expérience de décennies de programmation orientée objet et proposait **23 solutions types** pour
des problèmes récurrents. Ces recettes, appelées **Design Patterns** (*patrons de conception*), devinrent rapidement une
langue commune entre bâtisseurs, un vocabulaire de métier qui permettait aux architectes et aux développeurs de se
comprendre en quelques mots.

---

## Les trois familles de patterns

Le grimoire divisait ses enseignements en trois grandes familles, comme trois ordres de chevalerie :

- Les **créationnels**, qui enseignaient l’art d’engendrer des objets avec élégance.
- Les **structurels**, qui montraient comment composer et organiser les briques du royaume.
- Les **comportementaux**, qui réglaient les interactions et les responsabilités entre habitants de la cité-logiciel.

---

## Les patterns de création – les ateliers d’objets

Les patterns de création étaient les ateliers secrets où l’on façonnait les nouveaux habitants du royaume.

- **Singleton** : un roi unique qui garantit qu’il n’existe qu’une seule instance. Utile pour les journaux d’événements
  ou les configurations globales, mais tyrannique lorsqu’il s’impose partout.
- **Factory Method** : un atelier discret qui fabrique les objets sans dévoiler leurs secrets. On délègue la création et
  l’on centralise les variantes.
- **Abstract Factory** : une guilde entière d’ateliers, capables de produire des familles cohérentes d’objets adaptés à
  un même univers (par exemple, des boutons et fenêtres pour Windows, Mac ou Linux).
- **Builder** : le maître d’œuvre qui érige une construction complexe par étapes, comme un architecte dirigeant la
  construction d’une cathédrale.
- **Prototype** : l’artisan du moulage : plutôt que de repartir de zéro, on clone un modèle existant et on le
  personnalise, comme un potier utilisant un moule.

---

## Les patterns structurels – les tailleurs de pierre

Ces patterns montraient comment assembler les pierres pour bâtir des édifices cohérents et solides.

- **Adapter** : le traducteur qui permet à deux interfaces incompatibles de collaborer, comme un interprète entre deux
  peuples.
- **Bridge** : le séparateur de pouvoirs. Il dissocie l’abstraction de son implémentation, afin qu’elles puissent
  évoluer indépendamment, tel un pont reliant deux rives sans les figer.
- **Composite** : l’organisateur d’arbres. Il permet de traiter de la même façon les branches et les feuilles, comme
  dans une bibliothèque où livres et rayons obéissent à la même logique.
- **Decorator** : le tailleur d’habits. Il enrobe un objet de nouveaux atours (comportements) sans toucher à son corps.
- **Facade** : la grande porte d’un château, qui simplifie l’accès à un système complexe en offrant une entrée unique.
- **Flyweight** : l’économe, qui partage les ressources légères pour économiser de la mémoire, comme une imprimerie
  réutilisant les mêmes caractères.
- **Proxy** : le majordome qui se tient devant la porte et contrôle l’accès à l’objet qu’il protège.

---

## Les patterns comportementaux – les maîtres des interactions

Ces patterns régissaient la vie quotidienne de la cité-logiciel, les dialogues, les alliances et les rituels.

- **Observer** : le crieur public. Quand un événement survient, il alerte immédiatement tous ceux qui écoutent.
  Exemple : un modèle qui notifie ses vues dans MVC.
- **Strategy** : le général d’armée. Il permet de choisir et d’interchanger les tactiques en fonction du champ de
  bataille.
- **Command** : le parchemin scellé. Chaque action devient un objet que l’on peut transmettre, archiver ou rejouer plus
  tard.
- **Chain of Responsibility** : la chaîne de scribes. Une requête circule de l’un à l’autre jusqu’à trouver celui qui
  saura la traiter. Exemple : les middlewares HTTP.
- **Mediator** : le diplomate central. Il règle les échanges pour éviter que chaque objet ne doive parler directement à
  tous les autres.
- **Memento** : le gardien de mémoire. Il capture l’état d’un objet pour permettre de le restaurer plus tard.
- **State** : le métamorphe. Le comportement change selon l’état interne, comme une porte qui peut être ouverte, fermée
  ou verrouillée.
- **Template Method** : le livre de recettes. Il définit un cadre fixe pour un algorithme, laissant à des sous-classes
  le soin de remplir certaines étapes.
- **Visitor** : le voyageur curieux. Il parcourt une structure et applique une opération à chaque élément, sans modifier
  la structure elle-même.
- **Interpreter** : le linguiste. Il définit une grammaire et un interprète pour comprendre un langage spécialisé.
- **Iterator** : le guide touristique. Il permet de visiter une collection élément par élément, sans exposer son
  organisation interne.

---

## Les bonnes pratiques en renfort

Les patterns ne vivaient pas seuls : ils s’accompagnaient de règles de sagesse, gravées par les bâtisseurs pour éviter
les excès.

- **KISS (Keep It Simple, Stupid)** : la simplicité reste la première qualité d’une architecture. Trop de complexité
  mène à la chute.
- **Law of Demeter (1987)** : “Don’t talk to strangers.” Un objet ne doit pas dialoguer avec des inconnus par des
  chaînes d’appels interminables.
- **Open/Closed Principle (1988, Bertrand Meyer)** : un logiciel doit être ouvert à l’extension, mais fermé à la
  modification. On enrichit l’existant sans briser les murs.
- **YAGNI (You Ain’t Gonna Need It)** : issu de l’**Extreme Programming**. Ne bâtis pas une tour dont personne n’a
  besoin. Construis ce qui est nécessaire, rien de plus.
- **Hollywood Principle** : “Don’t call us, we’ll call you.” Principe des frameworks : c’est l’ossature qui décide quand
  invoquer ton code.
- **SOLID (Robert C. Martin, années 2000)** : un acronyme qui formalisa cinq principes déjà présents dans l’air du
  temps :
    - **Single Responsibility** : chaque classe ne doit avoir qu’une seule raison de changer.
    - **Open/Closed** : déjà évoqué, l’art d’étendre sans modifier.
    - **Liskov Substitution** : une sous-classe doit pouvoir remplacer sa super-classe sans altérer le comportement
      attendu.
    - **Interface Segregation** : mieux vaut plusieurs petites interfaces cohérentes qu’une énorme façade lourde.
    - **Dependency Inversion** : les modules de haut niveau ne dépendent pas des détails, mais d’abstractions stables.

Ces principes formaient une **constitution pratique** du royaume, des garde-fous pour éviter que les édifices ne
s’effondrent sous le poids de leur propre complexité.

---

## Le revers des patterns

Mais le succès du grimoire eut un prix.  
Certains apprentis, fascinés par la beauté des patterns, voulurent les appliquer partout, même là où une simple
fonction suffisait. On vit fleurir des codes où chaque addition passait par une Factory, où le plus petit objet se
voyait décoré de couches inutiles.

Cet excès fut baptisé **overengineering** : l’art de compliquer un problème simple.  
Comme des écuyers en armure complète envoyés chercher du pain, ces projets impressionnaient mais manquaient
cruellement d’efficacité.

---

## Anecdotes et héritage

- Le livre du Gang of Four devint une **Bible universitaire** : impossible de suivre un cours d’informatique dans les
  années 2000 sans croiser le Singleton, l’Observer ou le Factory.
- Dans les entretiens techniques, il était courant d’entendre : *“Citez trois patterns et expliquez-les.”*
- Certains langages modernes (Python, Ruby, Scala) intégrèrent directement des idiomes qui rendaient certains patterns
  superflus, mais le vocabulaire resta.
- Des héritiers prolongèrent la tradition : **Enterprise Patterns** (Martin Fowler, 2002), puis les **Cloud Patterns**
  et enfin les **Microservices Patterns**, adaptés aux nouveaux contextes.

---

## Métaphore finale

Les Design Patterns furent comme des **contes initiatiques**, transmis de maître à élève.  
Chacun contenait une morale, une solution éprouvée pour un problème typique. Mais mal compris, ces récits pouvaient
devenir des mythes superstitieux, appliqués sans discernement.

> Un pattern est un outil précieux, mais il ne sert que si le problème existe réellement.

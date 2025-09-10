# Chapitre VI – Les Patterns des Sages (1994 et après)

![chapitre VI.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-VI.png)

En **1994**, quatre conteurs surnommés le **Gang of Four** – **Erich Gamma**, **Richard Helm**, **Ralph Johnson** et
**John Vlissides** – publièrent un grimoire qui allait marquer l’histoire du développement logiciel :  
**Design Patterns: Elements of Reusable Object-Oriented Software**.

Ce livre condensait l’expérience de décennies de programmation orientée objet et proposait **23 solutions types** pour
des problèmes récurrents. Ces recettes, appelées **Design Patterns** (*patrons de conception*), devinrent une langue
commune pour les architectes et développeurs.

---

## Les trois familles de patterns

Les patterns du Gang of Four se répartissaient en trois grandes familles, comme trois ordres de chevalerie :

- **Créationnels** : comment instancier proprement des objets.
- **Structurels** : comment organiser et composer des objets.
- **Comportementaux** : comment gérer les interactions et responsabilités.

---

## Les patterns de création – les ateliers d’objets

1. **Singleton** : un roi unique, qui garantit qu’une seule instance existe. Exemple : un *logger* ou une configuration
   globale. Puissant mais tyrannique s’il est trop utilisé.
2. **Factory Method** : un atelier qui fabrique des objets sans révéler les détails de leur construction. Permet de
   déléguer la création et de centraliser les variantes.
3. **Abstract Factory** : un atelier de luxe qui fabrique non pas un objet, mais **toute une famille cohérente** (ex. :
   widgets pour Windows, Mac ou Linux).
4. **Builder** : un maître d’œuvre qui construit un objet étape par étape, comme un architecte qui dirige la
   construction
   d’une cathédrale. Exemple : créer un document complexe en plusieurs phases.
5. **Prototype** : plutôt que de repartir de zéro, on clone un modèle existant et on le personnalise. Comme un artisan
   qui part d’un moule.

---

## Les patterns structurels – les tailleurs de pierre

1. **Adapter** : un traducteur qui permet à deux interfaces incompatibles de collaborer, comme un guide bilingue.
2. **Bridge** : séparer une abstraction de son implémentation, comme séparer la télécommande de la télévision.
3. **Composite** : organiser des objets en arbre hiérarchique (ex. : dossiers et fichiers), où chaque feuille et chaque
   branche se manipule de la même façon.
4. **Decorator** : un tailleur qui habille les objets avec de nouveaux vêtements (comportements) sans toucher à leur
   corps. Exemple : ajouter un *scrollbar* à une fenêtre.
5. **Facade** : la grande porte d’entrée d’un château, qui simplifie l’accès à un système complexe en exposant une
   interface unique.
6. **Flyweight** : partager des objets légers pour économiser de la mémoire, comme une imprimerie réutilisant les mêmes
   caractères typographiques.
7. **Proxy** : un intermédiaire qui contrôle l’accès à un objet, comme un majordome filtrant les visiteurs.

---

## Les patterns comportementaux – les maîtres des interactions

1. **Observer** : un crieur public avertit aussitôt toute la ville lorsqu’un événement survient. Exemple : le modèle qui
   notifie toutes les vues dans MVC.
2. **Strategy** : un général choisit la tactique adaptée au champ de bataille. Exemple : différents algorithmes de tri.
3. **Command** : transformer une action en objet (ex. : “Undo” dans un éditeur). Les ordres deviennent des parchemins
   archivables.
4. **Chain of Responsibility** : une requête circule dans une chaîne de scribes jusqu’à trouver celui qui sait la
   traiter. Exemple : middleware HTTP.
5. **Mediator** : un diplomate centralise les échanges entre objets, évitant que tous parlent directement entre eux.
6. **Memento** : conserver un état passé comme une photo-souvenir, pour revenir en arrière. Exemple : points de
   restauration.
7. **State** : un automate qui change de comportement selon son état (porte ouverte, fermée, verrouillée).
8. **Template Method** : une recette de cuisine avec des étapes fixes, mais certaines étapes sont laissées à la liberté
   du chef.
9. **Visitor** : un voyageur qui traverse une structure et applique une opération spécifique à chaque élément, sans
   modifier la structure elle-même.
10. **Interpreter** : construire un langage miniature avec sa propre grammaire et interpréteur. Exemple : expressions
    mathématiques.
11. **Iterator** : un guide qui permet de visiter une collection sans en exposer les détails internes.

---

## Les bonnes pratiques en renfort

Les patterns ne vivaient pas seuls : ils s’inscrivaient dans une culture grandissante de **bonnes pratiques** :

- **KISS (Keep It Simple, Stupid)** : rappeler que la simplicité est la première qualité d’une architecture.
- **Law of Demeter (1987)** : *“Don’t talk to strangers”*, éviter les longues chaînes d’appels pour limiter le couplage.
- **Open/Closed Principle (1988, Bertrand Meyer)** : *ouvert à l’extension, fermé à la modification*.
- **YAGNI (You Ain’t Gonna Need It)** : issu de l’**Extreme Programming** (années 90), mettre en garde contre le code
  anticipé inutile.
- **Hollywood Principle** : *“Don’t call us, we’ll call you”*, principe des frameworks qui imposent leur cycle de vie.
- **SOLID (Robert C. Martin, années 2000)** : un acronyme qui formalisa et popularisa cinq principes déjà dans l’air du
  temps.

Ces règles formaient une sagesse pratique : des garde-fous contre la tentation de transformer chaque programme en
encyclopédie de patterns.

---

## Le revers des patterns

Le succès des patterns eut un prix. Certains apprentis, fascinés par le grimoire, voulurent les appliquer partout, même
là où une simple fonction suffisait. On vit apparaître des codes où la moindre addition passait par une *Factory* et un
*Decorator*, alourdissant inutilement les projets.

On appela cela l’**overengineering** : l’art de compliquer un problème simple. Comme des chevaliers en armure complète
partant acheter du pain, ces projets impressionnaient mais manquaient d’efficacité.

---

## Anecdotes et héritage

- Le livre du Gang of Four devint une **Bible universitaire** : impossible de suivre un cours d’informatique dans les
  années 2000 sans entendre parler du Singleton ou de l’Observer.
- Les entretiens techniques demandèrent souvent : *“Citez trois patterns et expliquez-les”*, preuve de leur diffusion
  culturelle.
- Certains langages modernes (Python, Ruby, Scala) intégrèrent directement des idiomes qui rendaient certains patterns
  superflus, mais le vocabulaire resta.
- Des dérivés virent le jour : **Enterprise Patterns** (Martin Fowler, 2002), **Cloud Patterns**, **Microservices
  Patterns**, prolongeant la tradition.

---

## Métaphore finale

Les Design Patterns furent comme des **contes initiatiques** transmis de maître à élève. Chaque histoire contenait une
morale, une solution éprouvée pour un problème typique. Mais mal interprétés, ces contes pouvaient tourner au mythe
superstitieux.

> Un pattern est un outil précieux, mais il ne sert que si le problème existe réellement.

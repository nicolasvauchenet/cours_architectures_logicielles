# Chapitre III – L’Ordre des Objets (années 80–90)

![chapitre III.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-III.png)

Au tournant des années 80, un vent d’organisation souffla sur l’informatique. Les bâtisseurs de code, fatigués de
manipuler des structures linéaires et rigides, rêvèrent d’un monde où les programmes seraient peuplés de petites entités
autonomes, dialoguant entre elles comme des citoyens dans une cité bien ordonnée. Ces entités reçurent un nom qui allait
marquer durablement l’histoire : **les objets**.

---

## Alan Kay et la philosophie des objets

Le visionnaire **Alan Kay**, travaillant au Xerox PARC, forgea dès le début des années 70 l’idée de **Smalltalk**.  
Son intuition était simple et puissante : un programme devrait ressembler à une société d’agents. Chaque agent — ou
objet — possède une **identité**, des **responsabilités** et des **comportements**, et il communique avec les autres par
des messages.

Smalltalk, apparu en **1980**, fut plus qu’un langage : c’était un laboratoire d’idées. Il introduisit la programmation
orientée objet (POO) comme une philosophie. Kay lui-même disait :

> « L’essence de l’objet est de combiner le comportement et l’état, et de masquer les détails inutiles. »

Dans les laboratoires de Palo Alto, les chercheurs manipulaient déjà des interfaces graphiques à la souris sur des
machines Xerox Alto, programmées en Smalltalk — préfigurant les ordinateurs personnels modernes.

---

## Bjarne Stroustrup et la naissance de C++

Pendant ce temps, à **Bell Labs**, **Bjarne Stroustrup** cherchait à enrichir la puissance du langage C. En **1985**, il
publia la première version de **C++**, qui introduisait les classes, l’héritage et les objets, tout en conservant la
vitesse et le contrôle du C.

C++ fut adopté massivement dans l’industrie, en particulier pour le développement de systèmes critiques, de logiciels
scientifiques et de jeux vidéo. Des moteurs graphiques aux bases de données, C++ devint le cheval de bataille de toute
une génération.

> « C++ rend les structures grandes et complexes plus faciles à comprendre et à maintenir. »  
> — Bjarne Stroustrup, *The C++ Programming Language* (1985)

Mais avec cette puissance venait la complexité. La gestion de la mémoire restait manuelle, et la syntaxe, lourde,
effrayait parfois les nouveaux venus.

---

## James Gosling et la promesse de Java

En **1995**, chez Sun Microsystems, **James Gosling** et son équipe inventèrent **Java**. Le slogan fit rêver les
développeurs : *“Write once, run anywhere”*. Grâce à sa **machine virtuelle (JVM)**, un programme Java pouvait être
écrit une fois et exécuté sur n’importe quelle machine, du PC au serveur, sans modification.

Java apportait aussi une **gestion automatique de la mémoire** via le *garbage collector*, réduisant les erreurs liées
aux pointeurs qui hantaient C et C++. Rapidement, Java devint le langage des applications d’entreprise, des systèmes
bancaires et des premiers serveurs web dynamiques.

Anecdote : le langage devait initialement s’appeler *Oak*, en référence à un chêne devant le bureau de Gosling. Mais le
nom était déjà pris ; l’équipe choisit finalement “Java”, inspiré du café indonésien qu’ils buvaient en continu.

---

## Les trois piliers de l’objet

La programmation orientée objet se résumait à trois principes cardinaux :

1. **Encapsulation** : cacher l’intérieur des objets et ne révéler qu’une interface publique, comme une boîte noire dont
   on ne connaît que les boutons.
2. **Héritage** : organiser les objets en familles et permettre à une classe “enfant” de réutiliser les comportements
   d’une classe “parent”.
3. **Polymorphisme** : un même message envoyé à différents objets peut produire des réactions différentes, comme une
   même question posée à plusieurs personnes qui donneront chacune une réponse unique.

Ces principes donnaient aux logiciels une modularité et une réutilisabilité inédites. On pouvait désormais bâtir des
**bibliothèques réutilisables** et des **cadres de développement** (frameworks), pierre angulaire des décennies
suivantes.

---

## Les premières règles de conduite

Avec la puissance nouvelle de la POO vinrent aussi ses excès : hiérarchies trop profondes, classes tentaculaires,
abstractions en cascade. Les pionniers comprirent vite qu’il fallait fixer des règles de bon sens, comme une charte pour
éviter que la cité des objets ne devienne un labyrinthe.

- **KISS (Keep It Simple, Stupid)** : emprunté à l’aéronautique (années 60), ce principe rappelait aux programmeurs que
  la simplicité reste la meilleure arme contre la complexité. Trop de classes et d’héritages, et le code se change en
  bureaucratie logicielle.
- **Law of Demeter (1987, Ian Holland)** : surnommée *“Don’t talk to strangers”*, elle recommandait qu’un objet parle
  uniquement à ses proches, pas à des inconnus via de longues chaînes d’appels. L’objectif : limiter le couplage et
  préserver l’autonomie de chaque objet.
- **Open/Closed Principle (1988, Bertrand Meyer)** : un logiciel doit être *ouvert à l’extension, mais fermé à la
  modification*. Autrement dit, on doit pouvoir enrichir une classe sans casser son code existant, un idéal incarné dans
  le langage **Eiffel**.

Ces règles étaient encore des balises isolées, mais elles annonçaient une formalisation croissante. Elles préfiguraient
le mouvement qui, une décennie plus tard, mènerait à l’acronyme **SOLID** et à toute une discipline de design logiciel.

---

## Les promesses et les dérives

Si la POO apportait de l’ordre, elle pouvait aussi devenir une **bureaucratie numérique**. Les développeurs, grisés par
les hiérarchies, créèrent parfois des arbres de classes si profonds que personne n’osait plus y toucher. Les projets
s’enlisaient dans des forêts d’abstractions, où une simple modification nécessitait de remplir des formulaires
conceptuels à chaque étage.

Certains critiques dirent que la POO, mal utilisée, produisait du “code spaghetti orienté objet”, où la réutilisation
promise se transformait en rigidité.

---

## Métaphore finale

On peut voir cette époque comme l’apparition des **villes médiévales fortifiées**. Chaque objet est une maison avec ses
portes (méthodes publiques) et ses murs (encapsulation). Les familles (héritage) organisent la cité, et les habitants
interagissent librement (polymorphisme).

Mais comme dans toute cité trop administrée, le risque est grand que les habitants passent plus de temps à respecter les
procédures qu’à bâtir des ponts.

> Les objets apportaient de l’ordre, mais risquaient de transformer les projets en bureaucraties compliquées.

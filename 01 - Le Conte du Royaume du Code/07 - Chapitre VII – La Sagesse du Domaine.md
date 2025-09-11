# Chapitre VII – La Sagesse du Domaine (2003)

![chapitre-VII.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-VII.png)

## Le Livre Bleu d’Eric Evans

En **2003**, un nouveau codex apparut dans le Royaume du Code : *Domain-Driven Design: Tackling Complexity in the Heart
of Software*.  
Son auteur, **Eric Evans**, un bâtisseur à la fois ingénieur et philosophe, y proposait une vision nouvelle.  
Ce n’était plus un livre de recettes techniques, mais une véritable **charte politique** : il plaçait le **métier** au
centre des préoccupations, et rappelait que le rôle du logiciel n’était pas de briller par sa complexité, mais
d’incarner fidèlement les réalités du monde qu’il servait.

À une époque où beaucoup d’édifices croulaient sous les frameworks, les EJBs et les couches techniques, Evans martela
une maxime devenue légendaire :
> « L’architecture doit servir le domaine, et non l’inverse. »

Son ouvrage, rapidement surnommé le **Livre Bleu**, fut perçu comme une révélation. Certains y virent un manuel austère,
d’autres une prophétie, mais tous reconnurent qu’il marquait un tournant majeur.

---

## Le langage ubiquitaire

Le premier enseignement du Livre Bleu fut l’idée du **langage ubiquitaire**.  
Trop souvent, les bâtisseurs parlaient en termes techniques — tables SQL, entités persistées, pointeurs — quand les
maîtres du métier parlaient d’autre chose : clients, contrats, transactions. Ces deux mondes se croisaient sans jamais
vraiment se comprendre.

Evans proposa une réconciliation : que le code et la parole humaine ne fassent plus qu’un.  
Dans une banque, le code devait contenir des *Comptes*, des *Transactions* et des *Clients*, plutôt que des “Tbl_Cust”
ou “Row42”.  
Le langage métier devenait une **lingua franca**, une langue commune parlée autant dans les salles de réunion que dans
les ateliers de développement.

Ce principe simple avait une portée énorme : il rapprochait deux castes qui s’étaient toujours méfiées l’une de
l’autre — les experts métier et les développeurs — et les unissait dans une même cité.

---

## Les provinces autonomes : les Bounded Contexts

Evans constata aussi que, dans les grandes organisations, un mot pouvait avoir plusieurs significations.  
Le mot “client” n’avait pas la même portée pour le département commercial, pour la logistique ou pour la comptabilité.  
Ce flou sémantique provoquait des guerres internes, des quiproquos, et des logiciels incohérents.

Pour résoudre cela, il proposa les **Bounded Contexts** : des frontières nettes et assumées, des **provinces autonomes**
du royaume, où chaque mot, chaque modèle avait une signification précise.  
Les contextes pouvaient ensuite établir des traités entre eux, appelés **Context Maps** : partenariats, alliances,
relations maître-esclave, ou simples relations de voisinage.  
Cette approche fit entrer la politique dans le logiciel : le royaume n’était plus un bloc homogène, mais une mosaïque de
provinces souveraines.

---

## Les briques du DDD

Au-delà de cette vision politique, le Livre Bleu proposa une **boîte à outils concrète** pour bâtir les cités
logicielles.

- Les **Entities**, citoyens définis par leur identité unique, qui survit aux changements d’état.
- Les **Value Objects**, objets sans identité, définis seulement par leur valeur : une date, une monnaie, une couleur.
- Les **Aggregates**, provinces internes qui regroupent plusieurs entités et valeurs sous une même autorité, la racine.
- Les **Repositories**, portes d’accès abstraites pour récupérer ou stocker les agrégats, cachant la lourdeur des bases
  de données.
- Les **Services**, qui incarnent des actions du domaine ne trouvant pas leur place ailleurs.

Ces briques étaient des **outils tactiques** pour organiser le code, mais aussi pour l’aligner sur le langage du métier.

---

## Onion et Clean : cathédrales concentriques du DDD

Pour donner une forme architecturale à ces principes, certains maîtres-bâtisseurs dessinèrent des plans de cathédrales
concentriques.

En **2008**, **Jeffrey Palermo** proposa l’**Onion Architecture**.  
Le domaine y était placé au centre, protégé par des couches en anneaux successifs : application, infrastructure,
interfaces.  
Les dépendances ne pouvaient qu’aller vers l’intérieur, jamais vers l’extérieur. Ainsi, on pouvait changer de base de
données ou de technologie sans menacer le cœur.  
Cette métaphore de l’oignon, avec ses pelures protectrices, séduisit ceux qui voulaient préserver le métier des assauts
du monde extérieur.

En **2012**, **Robert C. Martin** – *Uncle Bob* – popularisa la **Clean Architecture**, une déclinaison du même idéal.  
Ses cercles concentriques rappelaient l’Onion, mais il insista sur une règle cardinale : les dépendances doivent
toujours **pointer vers l’intérieur**.  
Au centre, on trouve les entités métier, puis les cas d’usage, puis les interfaces, et enfin, à l’extérieur, les
frameworks et outils.  
La Clean Architecture proclamait l’indépendance du logiciel vis-à-vis des outils éphémères.  
Le code devait “crier son domaine” (*Screaming Architecture*), être lisible et compréhensible même sans lire une seule
ligne technique.

Ces deux architectures, Onion et Clean, furent vues comme les **incarnations monumentales du DDD**, des cathédrales
logicielles où le métier trônait au sanctuaire central.

---

## Une cousine éloignée : l’Hexagonal Architecture

Une autre approche, contemporaine mais plus ancienne et moins concentrique, née sous la plume d’**Alistair Cockburn** y
trouva enfin sa raison d'exister : l’**architecture hexagonale**, aussi appelée **Ports & Adapters** (2005).  
Passée jusqu'alors un peu inaperçue, elle fut redécouverte grâce au DDD.  
Plutôt que des cercles, Cockburn dessinait un hexagone.
Le domaine restait au centre, mais les relations avec le monde extérieur passaient par des ports (contrats) et des
adaptateurs (implémentations concrètes).

Cette vision plus pragmatique s’adaptait bien aux projets agiles : l’hexagone n’imposait pas de grandes cathédrales
concentriques, mais offrait des façades multiples, ouvertes sur différents mondes (bases de données, interfaces web, API
externes).  
C’était une **cousine éloignée** du DDD, partageant le même idéal de protection du métier, mais avec une forme
géométrique plus souple et plus adaptée aux batailles quotidiennes.

---

## Les traités diplomatiques : CQRS et Event Sourcing

La pensée d’Evans inspira aussi de nouvelles pratiques pour gérer les cités distribuées.

- Le **CQRS (Command Query Responsibility Segregation)**, popularisé par **Greg Young**, séparait les chemins : d’un
  côté les commandes (qui modifient l’état), de l’autre les requêtes (qui consultent).
- L’**Event Sourcing** proposait de ne pas stocker seulement l’état final, mais l’ensemble des événements passés.  
  Ainsi, un logiciel devenait une **chronique historique**, où chaque fait était consigné, permettant de rejouer
  l’histoire ou de reconstituer des scénarios.

Ces traités diplomatiques apportèrent une profondeur temporelle au code, transformant les applications en annales
vivantes.

---

## Les avantages et les limites

La Sagesse du Domaine apporta une vision claire : replacer le métier au centre, clarifier les frontières, donner un
langage commun et des architectures protectrices.  
Elle inspira profondément les communautés **Java** et **.NET**, où les frameworks se multiplièrent pour appliquer ces
concepts.

Mais cette sagesse avait aussi ses dangers.  
Le Livre Bleu était dense et intimidant, et certains bâtisseurs s’y perdirent.  
D’autres, fascinés par les cercles concentriques, sombrèrent dans un excès d’abstraction, multipliant couches et modèles
sans jamais livrer un logiciel utile.  
La promesse d’aligner le code et le métier pouvait ainsi tourner au carcan paralysant.

---

## Moralité

La Sagesse du Domaine fut une révolution culturelle autant que technique.  
Elle rappela que le logiciel n’est pas une fin en soi, mais un miroir fidèle du monde qu’il sert.  
Les provinces autonomes (Bounded Contexts), les cathédrales concentriques (Onion et Clean), les polygones pragmatiques (
Hexagonal), et les traités diplomatiques (CQRS, Event Sourcing) composèrent une nouvelle ère d’architecture.

> Le domaine est le cœur vivant du logiciel : toutes les architectures qui l’entourent ne sont que des fortifications
> pour le protéger.

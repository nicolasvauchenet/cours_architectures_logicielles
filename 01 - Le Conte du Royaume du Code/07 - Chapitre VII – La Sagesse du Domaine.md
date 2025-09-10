# Chapitre VII – La Sagesse du Domaine (2003)

![chapitre VII.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-VII.png)

En **2003**, un nouveau maître fit son apparition : **Eric Evans**. Son ouvrage bleu, sobrement intitulé *Domain-Driven
Design: Tackling Complexity in the Heart of Software*, allait devenir une référence pour tous ceux qui luttaient contre
la complexité grandissante des systèmes.

Sa philosophie était limpide : **l’architecture devait servir le métier, et non l’inverse**. Là où beaucoup de projets
étaient engloutis dans des couches techniques, Evans rappelait que la véritable valeur résidait dans le *domaine*,
c’est-à-dire la connaissance métier que le logiciel devait incarner.

---

## Le langage du métier

Evans proposa une règle d’or : les développeurs et les experts métiers devaient partager un **langage commun**. Ce
*Ubiquitous Language* permettait d’éviter les malentendus et de faire en sorte que le code reflète exactement les termes
du métier.

Un exemple : dans une banque, on ne parle pas d’“enregistrement” ou de “table SQL”, mais de “compte”, de “transaction”,
de “client”. Le code devient ainsi une **représentation fidèle de la réalité métier**.

> « Si le langage du code ne correspond pas au langage du domaine, le fossé se creuse entre développeurs et experts. »  
> — Eric Evans, 2003

---

## Les Bounded Contexts – dessiner des frontières

Un système complexe est rarement uniforme. Evans introduisit la notion de **Bounded Contexts** : des zones clairement
délimitées où un langage et un modèle métier s’appliquent.

- Dans une entreprise, le contexte “Facturation” n’utilise pas les mêmes termes que le contexte “Logistique”.
- Chaque contexte définit son propre vocabulaire, ses règles et ses entités, évitant ainsi la confusion et les
  collisions
  sémantiques.

Les Bounded Contexts sont comme des **provinces autonomes** dans un royaume logiciel, chacune avec ses lois, mais
reliées
par des traités et des passerelles.

---

## Les briques du DDD

Evans proposa des briques conceptuelles pour structurer la logique :

- **Entities** : objets définis par leur identité (un client reste le même même si son adresse change).
- **Value Objects** : objets définis uniquement par leurs valeurs (une adresse, une date, une monnaie).
- **Aggregates** : ensembles cohérents d’objets, protégés par une racine qui contrôle leur intégrité.
- **Repositories** : portes d’accès aux agrégats, abstractions qui cachent la mécanique de persistance.
- **Services** : opérations métier qui ne trouvent pas naturellement leur place dans une entité ou un objet valeur.

Ces concepts donnèrent aux développeurs une **boîte à outils structurée** pour transformer un chaos d’objets en une
cité logique bien ordonnée.

---

## CQRS et Event Sourcing – les héritiers

La pensée d’Evans inspira d’autres sagesses :

- **CQRS (Command Query Responsibility Segregation)**, popularisé par Greg Young, qui recommande de séparer les
  commandes
  (qui modifient l’état) des requêtes (qui lisent l’état).
- **Event Sourcing**, qui propose de stocker non pas seulement l’état actuel, mais la **suite des événements** qui y ont
  conduit. Un système devient alors une chronique fidèle de tout ce qui s’est produit.

Ces mouvements prolongèrent la vision du DDD et influencèrent durablement les architectures distribuées et les
microservices des années suivantes.

---

## Anecdotes et héritage

- Le livre bleu d’Evans était d’abord perçu comme dense et théorique, mais il devint vite un **classique enseigné dans
  les conférences**.
- Le terme *“DDD”* devint un mot de passe entre initiés, un signe de reconnaissance dans les cercles d’architectes.
- La pensée DDD fut adoptée massivement par les communautés **Java** et **.NET**, puis influença l’écosystème
  **open source**.

---

## Un mouvement frère : l’architecture hexagonale

Au même moment, d’autres penseurs cherchaient à traduire cette sagesse du domaine en une **forme architecturale
précise**. En **2005**, **Alistair Cockburn** proposa l’**Architecture Hexagonale**, aussi appelée *Ports & Adapters*.

Son idée : placer le **domaine** au centre, protégé de toute dépendance technique. Autour de lui, des **ports**
définissent
les contrats d’entrée et de sortie (commandes, requêtes, événements), tandis que des **adapters** concrets les
implémentent (base de données, API externe, interface utilisateur).

Ce modèle, en apparence géométrique, répondait au même besoin qu’Evans : éviter que le code métier soit noyé sous les
détails d’infrastructure. On pouvait remplacer une base SQL par une base NoSQL, ou une interface console par une API
REST, sans toucher au cœur.

L’hexagone et le DDD étaient deux faces d’une même médaille :

- Evans donnait les **mots et les concepts** pour décrire le métier.
- Cockburn offrait une **forme et une discipline** pour préserver ce métier dans le code.

---

## Métaphore finale

La démarche d’Evans fut celle d’un **cartographe du sens**. Celle de Cockburn, celle d’un **architecte bâtisseur** qui
érigea des murailles hexagonales autour du domaine pour le protéger des assauts du monde extérieur.

> Le domaine est le cœur vivant du logiciel : tout le reste doit s’y adapter.

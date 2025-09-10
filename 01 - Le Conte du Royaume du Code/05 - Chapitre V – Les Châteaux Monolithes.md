# Chapitre V – Les Châteaux Monolithes (années 90–2000)

![chapitre V.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-V.png)

À mesure que l’industrie logicielle grandissait, les entreprises réclamèrent des systèmes toujours plus vastes :
**ERP (Enterprise Resource Planning)** pour gérer les processus internes, **CRM (Customer Relationship Management)**
pour centraliser les clients, et bientôt les premiers **sites d’e-commerce**. On bâtit alors des **Monolithes** :
de gigantesques châteaux regroupant toutes les fonctions sous un même toit, déployés en un seul bloc.

---

## Les Monolithes organisés

Un monolithe n’était pas nécessairement un tas informe de code. Les architectes de l’époque cherchèrent à imposer un
ordre intérieur, à l’image des citadelles médiévales organisées en quartiers.

- L’**architecture en couches (layered)** sépara clairement la **présentation** (interfaces et écrans), la **logique
  métier** (processus, calculs, règles), et les **données** (bases relationnelles, fichiers).
- L’**architecture n-tiers**, souvent déclinée en trois parties (UI, logique, base de données), devint le standard
  universellement enseigné et appliqué dans les universités et les écoles d’ingénieurs.

En pratique, cela signifiait qu’on déployait toujours **une seule application**, mais que son code interne était mieux
structuré. La couche de présentation (JSP, servlets, ASPX, pages PHP) communiquait avec une couche métier (EJB, Spring,
.NET), qui elle-même s’appuyait sur une couche d’accès aux données (JDBC, ADO.NET, ODBC).

---

## Langages et outils de l’époque

Chaque château monolithique se construisait avec des matériaux phares de l’époque :

- **Java (J2EE)** : né en 1995, il devint le langage-roi des architectures d’entreprise. EJB (Enterprise Java Beans),
  JSP et servlets peuplaient les tours et les remparts.
- **C# .NET** : lancé par Microsoft en 2000, il proposait une alternative moderne, intégrée à l’écosystème Windows.
- **PHP (1995)** : au départ un simple “Personal Home Page”, il évolua vite vers la création de sites dynamiques.
- **Perl** et **Ruby** : utilisés dans les scripts et dans certains frameworks naissants.

Les frameworks consolidèrent cette ère :

- **Spring (2003)** : apporta une gestion simplifiée des dépendances et un contrepied léger aux EJB lourds.
- **ASP.NET (2002)** : donna une structure forte aux applications web côté Microsoft.

Cette normalisation donna aux bâtisseurs une vraie grammaire commune pour édifier leurs forteresses numériques.

---

## Les atouts du monolithe

Le monolithe avait plusieurs qualités qui expliquent sa domination :

- **Cohérence interne** : toutes les fonctionnalités vivaient dans la même enceinte, avec une logique unifiée.
- **Déploiement simple** : une seule application à installer, à maintenir, à faire évoluer.
- **Outils centralisés** : logging, sécurité, transactions — tout était géré au même endroit.

Comme une forteresse, le monolithe protégeait son domaine derrière des murailles solides.

---

## Les limites et les failles

Mais la solidité du monolithe se payait en rigidité :

- Modifier une seule “salle” du château impliquait souvent de redéployer tout l’édifice.
- Les équipes, en grandissant, se marchaient sur les pieds dans le même code source.
- La scalabilité était limitée : on pouvait agrandir les murs, mais difficilement séparer les quartiers.

De nombreux projets, en voulant étendre un monolithe, se retrouvèrent prisonniers de ce que l’on appelait déjà
l’**effet big ball of mud** — la grosse boule de boue, où les couches s’entremêlent jusqu’à devenir indémêlables.

---

## Anecdotes et héritage

- Le logiciel **SAP R/3** (1992) incarna le modèle ERP monolithique, utilisé par des milliers d’entreprises à travers le
  monde.
- Les premiers sites d’e-commerce, comme **Amazon (1995)**, démarrèrent sur une base monolithique avant de migrer bien
  plus tard vers des architectures distribuées.
- Dans les universités, les étudiants de l’époque dessinaient fièrement les diagrammes “3-tiers” au tableau, symbole
  d’un savoir-faire professionnel.

---

## Métaphore finale

Les monolithes furent les **châteaux forts de l’ère logicielle**. Ils offraient protection, stabilité et unité. Mais
comme les châteaux médiévaux, ils devinrent difficiles à agrandir sans fissurer leurs murs.

> Le monolithe était fort et stable, mais manquait cruellement de souplesse.

# Chapitre V – Les Châteaux Monolithes (années 90–2000)

![chapitre-V.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-V.png)

## L’essor des forteresses

À mesure que le Royaume du Code grandissait, les royaumes marchands réclamèrent des systèmes toujours plus vastes.  
Les bâtisseurs ne se contentèrent plus de simples cités-objets : ils édifièrent d’immenses **châteaux monolithes**,
capables d’abriter toutes les fonctions sous un même toit.

Les plus célèbres de ces forteresses furent les **ERP (Enterprise Resource Planning)**, pour gérer la production et les
flux internes, les **CRM (Customer Relationship Management)**, pour centraliser les clients, et les premiers sites
d’**e-commerce** qui ouvraient de nouvelles routes marchandes numériques. Dans ces châteaux, chaque salle avait son
usage, chaque aile son rôle, mais l’ensemble formait un seul et unique bloc.

---

## Les couches et les quartiers

Un château monolithique n’était pas nécessairement un amas désordonné de pierre. Les architectes de l’époque imposèrent
des règles pour organiser l’intérieur.  
Ainsi naquirent les architectures **en couches** : présentation en façade, logique métier dans les grandes salles
centrales, et bases de données enterrées dans les caves profondes.

La variante **n-tiers**, souvent en trois parties (interface, logique, données), fut enseignée comme un dogme dans les
universités et adoptée par toutes les grandes guildes.  
Dans les amphithéâtres des années 90, des générations d’étudiants apprenaient à tracer au tableau le schéma sacré des
**“trois couches”**, comme un rite d’initiation qui symbolisait l’accès à la maîtrise logicielle.

---

## Les matériaux de l’époque

Les châteaux monolithes étaient bâtis avec les matériaux phares des années 90 et 2000 :

- **Java (J2EE)** : le langage-roi des architectures d’entreprise, peuplé d’**EJB** (Enterprise Java Beans), de **JSP**
  et de servlets.
- **C# .NET** : le chevalier de Microsoft, lancé en 2000, pour bâtir des forteresses intégrées à l’univers Windows.
- **PHP (1995)** : au départ une cabane bricolée, il devint vite une pierre souple pour ériger des sites dynamiques.
- **Perl** et **Ruby** : compagnons utiles pour sculpter des parties spécifiques de l’édifice.

Les frameworks furent les maîtres maçons de cette époque.  
**Spring (2003)** vint alléger les lourdeurs des EJB, apportant une injection de dépendances plus flexible.  
**ASP.NET (2002)** donna aux bâtisseurs Microsoft un socle puissant pour bâtir rapidement des applications web.

Et du côté du web grand public, on vit éclore des outils comme **JSP (Java Server Pages)** et **ASP (Active Server
Pages)**, qui permettaient de générer dynamiquement des pages web : de nouveaux ateliers intégrés aux murailles des
châteaux.

---

## Les seigneurs des monolithes

Certains châteaux devinrent de véritables empires.  
Le plus connu fut **SAP R/3 (1992)**, forteresse ERP adoptée par des milliers d’entreprises à travers le monde.  
Dans les terres marchandes d’outre-Atlantique, un marchand ambitieux nommé **Jeff Bezos** bâtit en 1995 son premier
site **Amazon**, fondé lui aussi sur une base monolithique. Ces forteresses prospéraient derrière leurs remparts,
imposant leur logique et leur puissance.

Mais les murailles trop épaisses pouvaient se retourner contre leurs habitants.  
**Netscape**, par exemple, s’enlisa dans une réécriture monumentale de son navigateur web, incapable de faire évoluer
son monolithe initial sans fissurer les murs. Cet échec ouvrit la voie au triomphe de Microsoft Internet Explorer dans
les années 90. Preuve que les forteresses, si elles se rigidifiaient trop, pouvaient condamner ceux qui y vivaient.

---

## Le spectre de la grosse boule de boue

Les châteaux monolithes avaient leurs ombres.  
À force de grandir, leurs murs devenaient trop épais et leurs couloirs labyrinthiques.  
Les bâtisseurs s’y marchaient sur les pieds, les dépendances s’entremêlaient, et l’édifice risquait de se transformer
en une **“grosse boule de boue”** (*big ball of mud*), où tout était lié à tout, et plus rien n’était compréhensible.

Modifier une seule salle exigeait parfois de reconstruire tout le château. La scalabilité était limitée : on pouvait
ajouter des pierres, mais difficilement séparer les quartiers sans fissurer les murs. Beaucoup d’entreprises se
retrouvèrent prisonnières de ces architectures massives, incapables de les faire évoluer sans douleur.

---

## Les avantages et les limites

Les châteaux monolithes avaient aussi des forces indéniables :  
ils offraient une **cohérence interne**, des **outils centralisés** (sécurité, transactions, logging) et un
**déploiement simple** — un seul artefact à installer, une seule forteresse à maintenir. Pour beaucoup d’organisations,
c’était un modèle rassurant, solide, presque féodal.

Mais leurs limites étaient tout aussi marquées :  
une **rigidité** qui freinait l’évolution, une **scalabilité** difficile, et une tendance à concentrer trop de
responsabilités dans un seul édifice.  
À mesure que les projets s’étendaient, la dette technique rongeait les murs comme une moisissure, menaçant l’équilibre
tout entier.

---

## Moralité

Les châteaux monolithes furent les forteresses du Royaume du Code : imposants, cohérents et protecteurs.  
Mais comme les châteaux médiévaux, ils devinrent difficiles à agrandir sans fissurer leurs murs.  
Leur force fut leur unité, mais leur faiblesse fut leur rigidité.  
Dans les salles des universités comme dans les tours des entreprises, les bâtisseurs comprirent que ce modèle, s’il
avait assuré leur gloire, préparait aussi leur prison.

> Le monolithe protégeait solidement ses habitants, mais il les enfermait aussi derrière ses propres murailles.

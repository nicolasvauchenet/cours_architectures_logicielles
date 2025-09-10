# Chapitre VIII – Les Villages de Microservices (années 2010)

![chapitre VIII.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-VIII.png)

Dans les années 2010, lassés des lourds Monolithes et de leurs murailles rigides, les bâtisseurs cherchèrent plus de
souplesse. Inspirés par des géants comme **Netflix**, **Amazon** ou **Spotify**, ils imaginèrent un nouveau modèle :
des villages composés de **microservices**.

Chaque maison de ce village avait son **métier propre**, communiquait avec ses voisines par des messages ou des APIs,
et pouvait être bâtie, réparée ou détruite sans menacer tout le village. C’était la promesse de l’agilité et de la
scalabilité à l’échelle d’Internet.

---

## Les pionniers des microservices

- **Amazon** : dès le milieu des années 2000, Jeff Bezos imposa que toutes les équipes développent des services
  communiquant uniquement par API. Ce décret fondateur devint la base de l’architecture d’AWS (Amazon Web Services).
- **Netflix** : confronté à une croissance exponentielle, l’entreprise passa d’un monolithe Java à une constellation de
  services indépendants. Elle inventa ou popularisa des outils comme **Hystrix** (pour le circuit breaker) et **Zuul**
  (pour l’API Gateway).
- **Spotify** : organisa ses équipes en “squads” autonomes, chacune responsable de ses microservices, incarnant la
  philosophie “you build it, you run it”.

Ces expériences inspirèrent toute une génération d’architectes.

---

## Les nouveaux patterns

Les villages distribués nécessitaient de nouvelles règles de vie :

- **API Gateway** : un portier unique qui gère l’entrée dans le village, centralise l’authentification et redirige vers
  les bonnes maisons.
- **Circuit Breaker** : un disjoncteur qui coupe un service en panne pour éviter qu’il n’entraîne toute la rue dans sa
  chute. Netflix popularisa ce pattern avec **Hystrix**.
- **Sidecar** : un petit compagnon attaché à chaque service, chargé de gérer les aspects transverses (logs, monitoring,
  sécurité). Ce principe donna naissance aux **Service Mesh** comme **Istio**.
- **Event-Driven Architecture** : plutôt que de s’appeler directement, les maisons du village pouvaient s’envoyer des
  messages asynchrones via un **bus d’événements** (Kafka, RabbitMQ).

Ces patterns permirent de dompter, au moins partiellement, la complexité du monde distribué.

---

## Les outils de l’ère microservices

- **Java Spring Boot (2014)** : simplifia la création d’applications Java prêtes à être déployées en microservices.
- **Node.js (2009)** : permit d’écrire des services légers et asynchrones en JavaScript, très adapté aux APIs.
- **Go (2009, Google)** : séduisit pour sa rapidité et sa simplicité dans l’écriture de services performants.
- **Docker (2013)** : révolutionna le déploiement en offrant des conteneurs isolés et reproductibles.
- **Kubernetes (2014, Google)** : orchestrait ces conteneurs comme un maire orchestre les infrastructures d’une ville.

Ces outils donnèrent aux bâtisseurs une flexibilité inédite : déployer 10, 100, voire 1000 microservices devint
possible.

---

## Les promesses et les périls

Les microservices apportaient :

- **Agilité** : chaque équipe pouvait avancer à son rythme, déployer son service indépendamment.
- **Scalabilité** : on pouvait multiplier les instances d’un service critique sans alourdir le reste.
- **Résilience** : une panne locale n’abattait pas tout le système.

Mais le prix à payer était lourd :

- **Complexité accrue** : surveiller, tester et coordonner des dizaines de services exigeait une discipline nouvelle.
- **Explosion des dépendances** : chaque maison devait savoir à quelle autre s’adresser, multipliant les contrats.
- **Bureaucratie de communication** : logs, monitoring, sécurité, orchestration — tout devait être repensé à l’échelle
  du village.

On vit apparaître le risque du **chaos organisé**, où la liberté se retournait contre elle-même.

---

## Héritage

Les microservices marquèrent un tournant :

- Ils inspirèrent l’essor du **DevOps**, où les équipes assument la responsabilité de leurs services en production.
- Ils préparèrent le terrain au **cloud computing**, où l’élasticité des infrastructures rendait leur modèle viable.
- Ils engendrèrent aussi des remises en question : certains prônèrent le retour à des **monolithes modulaires**,
  estimant que les microservices étaient un luxe réservé aux géants.

---

## Métaphore finale

Si le monolithe était un **château fort**, le monde des microservices ressemblait à un **village foisonnant** : chaque
maison autonome, chaque artisan indépendant. Mais un village mal coordonné risque vite de sombrer dans l’anarchie.

> Les microservices offraient la liberté, mais ils faisaient planer le risque d’un chaos organisé.

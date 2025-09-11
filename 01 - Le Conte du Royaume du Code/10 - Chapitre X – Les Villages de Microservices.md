# Chapitre X – Les Villages de Microservices (années 2010)

![chapitre-X.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-X.png)

## L’éclatement des forteresses

À l’orée des années 2010, certains bâtisseurs commencèrent à se lasser des **châteaux monolithes**.  
Ces forteresses étaient puissantes, mais leurs couloirs labyrinthiques ralentissaient chaque mouvement.  
Pour ajouter une simple salle, il fallait souvent rebâtir la moitié du château.  
Alors, quelques pionniers choisirent de briser ces murailles et de bâtir autrement : non plus une citadelle unique, mais
un **village d’artisans**.

Chaque maison de ce village possédait sa propre forge, son propre foyer, son rythme autonome.  
Ces maisons n’étaient pas isolées : elles échangeaient entre elles par des routes pavées de **messages** et
d'**API**.  
Ainsi naquit l’ère des **microservices**.

---

## Les pionniers : Amazon, Netflix, Spotify

Les premiers à expérimenter cette nouvelle urbanisation furent les grands marchands du Web.

**Amazon**, dont le château monolithique devenait ingérable, décida d’imposer une loi radicale : chaque équipe devait
exposer ses fonctionnalités via des **API claires**, accessibles aux autres comme à des clients externes. Cette
décision, attribuée à **Jeff Bezos**, fut le ferment de la culture des microservices.

**Netflix**, en quête de résilience pour son empire du streaming, adopta aussi cette organisation. Chaque microservice
devint une maison spécialisée : gestion des films, recommandations, paiements. Quand une maison tombait en ruine, les
autres continuaient à fonctionner.

**Spotify** popularisa l’image des **squads** et **tribus**, équipes autonomes responsables de leur propre service,
illustrant parfaitement l’esprit villageois. Leur cri de ralliement était :

> You build it, you run it.

---

## Les gardiens des routes

Dans ces villages, chaque maison avait un rôle clair, mais il fallait réguler le trafic entre elles.  
On mit en place des **API Gateways**, véritables gardiens des routes, qui contrôlaient qui pouvait entrer et sortir,
filtrant les messages et tenant des registres.

La communication passait par des rituels nouveaux : **REST** avec ses incantations HTTP, **gRPC** pour des dialogues
plus rapides, et les flux d’événements portés par **Kafka** ou **RabbitMQ**.  
Chaque maison devenait un petit royaume, avec sa forge logicielle, mais aussi son dialecte.

---

## Les catapultes modernes

Pour que ces villages prospèrent, il fallait de nouveaux outils de guerre.  
**Docker** apparut comme une arme magique : il enfermait chaque service dans un coffre étanche, transportable partout,
garantissant que le service tournerait de la même façon sur n’importe quelle machine.

Mais bientôt, les villages se multiplièrent à une telle échelle que leur gestion devint titanesque.  
Alors naquit **Kubernetes**, machine de siège moderne, capable d’orchestrer des armées entières de services, de les
déployer, de les cloner, de les ressusciter.  
Kubernetes devint le général des villages, tenant la carte de tout le territoire.

---

## Les promesses et les périls

Cette nouvelle organisation permit une agilité inédite.  
Chaque équipe pouvait construire, déployer et réparer sa maison sans attendre le bon vouloir du château central.  
La résilience s’en trouva accrue : si une maison brûlait, les autres continuaient d’assurer la vie du village.

Mais la complexité explosa.  
Les bâtisseurs passèrent de la gestion d’une forteresse unique à celle d’une myriade de chaumières bavardes.  
Les communications devinrent si nombreuses qu’une nouvelle **bureaucratie des messages** émergea : surveiller, tracer,
sécuriser, coordonner.  
Le rêve du village simple risquait de se transformer en une foire cacophonique, où l’énergie se perdait dans les
procédures.

---

## Moralité

Les microservices furent une révolution urbaine du Royaume du Code.  
Ils remplacèrent les châteaux lourds et rigides par des villages agiles et vivants.  
Mais ils rappelèrent aussi une leçon ancienne : multiplier les maisons n’élimine pas la complexité, elle la déplace.

> Le village des microservices prospère tant que ses routes sont claires et ses gardiens vigilants.  
> Mais livré au chaos des bavardages, il peut sombrer dans une cacophonie pire encore que les labyrinthes des
> monolithes.

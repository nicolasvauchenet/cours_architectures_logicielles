# Chapitre XI – Les Magiciens du Nuage (2015–2020)

![chapitre-XI.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-XI.png)

## L’arrivée des seigneurs du ciel

Après l’explosion des villages de microservices, le Royaume du Code leva les yeux vers le ciel.  
Au-dessus des terres encombrées de serveurs physiques et de salles des machines, de nouveaux seigneurs s’installèrent
dans les nuées. C'étaient les Magiciens du Nuage.  
Leurs noms résonnaient comme des incantations : **AWS (Amazon Web Services)**, **Microsoft Azure**, **Google Cloud
Platform (GCP)**.  
Chacun proposait aux bâtisseurs un marché étrange :
> Ne construisez plus vos propres forges.  
> Louez plutôt nos éclairs de calcul et nos rivières de stockage.  
> Payez à l’usage, et nous multiplierons vos forces.

Les châteaux et villages n’avaient plus besoin d’acheter des machines lourdes ni d’entretenir des caves climatisées
pleines de disques fragiles. Désormais, d’un claquement de doigts, on pouvait invoquer une armée de serveurs répartis
sur tous les continents.  
Cette promesse fascinait autant qu’elle inquiétait : pour la première fois, le pouvoir du calcul devenait aussi fluide
qu’un courant d’air.

---

## La magie serverless

Le plus étonnant des sortilèges apparut sous le nom de **serverless**.  
L’idée semblait paradoxale : il n’y avait plus besoin de serveurs visibles. En réalité, bien sûr, les machines
existaient toujours, mais elles étaient dissimulées dans les coulisses des magiciens.  
Le bâtisseur n’avait plus qu’à écrire une **fonction** – un sort court et précis – et à l’invoquer à volonté.

**AWS Lambda** (2014), **Azure Functions** et **Google Cloud Functions** popularisèrent cette magie.  
Les bâtisseurs y virent une liberté immense : plus de gestion d’infrastructure, seulement l’art pur de coder des
incantations.  
Mais la magie avait son prix : chaque invocation coûtait, et les factures grimpaient vite. Nombreux furent les royaumes
qui, croyant avoir trouvé la gratuité, se réveillèrent ruinés par la dîme cachée des magiciens.

---

## Les nouveaux rituels : CI/CD et Infrastructure as Code

Pour manier ces pouvoirs célestes, il fallut inventer de nouveaux rituels.  
Les bâtisseurs adoptèrent l’**Intégration Continue** et le **Déploiement Continu (CI/CD)**.  
Chaque fois qu’un artisan posait une nouvelle pierre (un commit), les prêtres du CI – **Jenkins**, **GitLab CI**,
**GitHub Actions**, **CircleCI** – déclenchaient leurs cloches.  
Ils testaient le code, le bénissaient, et s’il était jugé digne, ils l’envoyaient automatiquement vers les nuées.  
Ainsi, le cycle de construction s’accéléra : livraisons quotidiennes, parfois plusieurs fois par heure. Les anciens
rythmes mensuels parurent soudain archaïques.

Un autre art se développa : **l’Infrastructure as Code**.  
Plutôt que de configurer manuellement chaque serveur, les bâtisseurs écrivaient des grimoires décrivant toute leur
cité.  
**Terraform**, **CloudFormation**, **Ansible** permirent de recréer un royaume entier à l’identique, en Europe comme en
Asie, par la simple récitation d’un script.  
Cette magie de duplication fit naître l’ère des cités élastiques, capables de se déployer ou de disparaître à la vitesse
d’un orage.

---

## Les sentinelles et les oracles

Avec les microservices et le nuage, les cités logicielles devinrent immenses, mouvantes, insaisissables.  
Il ne suffisait plus de veiller sur quelques machines : il fallait surveiller des centaines, puis des milliers de
services.

De nouveaux oracles furent convoqués.  
**Prometheus** scrutait les métriques comme un devin lisant les étoiles.  
**Grafana** les projetait en fresques colorées sur de grandes cartes murales.  
Les bâtisseurs pouvaient ainsi anticiper les tempêtes, prévoir les pannes, déclencher des alertes.  
Jamais le Royaume du Code n’avait été autant surveillé – et jamais ses habitants ne s’étaient sentis aussi vulnérables,
conscients que la moindre alerte pouvait annoncer une catastrophe à grande échelle.

---

## Les fortunes et les désastres

De cette magie céleste naquirent des fortunes rapides.  
Des startups, sans un seul serveur physique, purent rivaliser avec des géants établis.  
On raconte que certaines entreprises bâtirent des empires en quelques mois, leurs seules armes étant une carte bancaire
et l’accès aux nuées d’AWS ou de GCP.

Mais les désastres furent tout aussi spectaculaires.  
Chaque panne d’un seigneur du ciel devenait un tremblement de terre.  
En **2017**, une simple faute de commande fit tomber une partie d’**AWS S3**, paralysant des centaines de sites à
travers le monde.  
En **2020**, une panne d’**Azure** plongea des milliers de clients dans le silence.  
On comprit alors que les royaumes du Code, autrefois isolés, étaient désormais liés par une même dépendance invisible :
si le nuage faiblissait, c’est le monde entier qui toussait.

---

## Le prix caché des sortilèges

Derrière ces miracles se cachait une dépendance inquiétante.  
Les royaumes, grisés par la facilité, confiaient leurs trésors aux seigneurs du ciel.  
Mais ces derniers fixaient leurs tarifs, et changer de nuage devenait une tâche titanesque.  
Les données étaient piégées dans des formats propriétaires, les services interconnectés de manière subtile.  
On appela cela le **vendor lock-in**, l’envoûtement invisible qui liait un royaume à son mage.

Le coût, d’abord modeste, se révélait parfois démesuré à grande échelle.  
Les bâtisseurs découvrirent que derrière chaque sortilège se cachait une dîme, et que la magie facile pouvait devenir
une dette écrasante.

---

## Moralité

Les Magiciens du Nuage ouvrirent une ère de prodiges.  
Ils permirent d’invoquer des armées de serveurs en un claquement de doigts, d’automatiser chaque rituel, de surveiller
les cités depuis les étoiles.  
Mais ils rappelèrent aussi une leçon ancienne : *nul pouvoir n’est gratuit*.  
Celui qui confie tout son royaume à un seigneur céleste doit accepter ses lois, ses tarifs et ses caprices.

> Les bâtisseurs du Code, fascinés par la magie du ciel, découvrirent que les chaînes invisibles du nuage peuvent être
> aussi lourdes que les murailles des anciens châteaux.  
> Car dans le Royaume du Code, toute lumière porte son ombre, et toute magie cache une dette.

# Chapitre IX – Les Magiciens du Nuage (2015–2020)

![chapitre IX.png](https://raw.githubusercontent.com/nicolasvauchenet/cours_architectures_logicielles/refs/heads/main/img/chapitre-IX.png)

À partir de 2015, les grands magiciens du **Cloud** – **Amazon AWS**, **Microsoft Azure** et **Google Cloud** –
s’imposèrent comme les nouveaux maîtres des infrastructures numériques. Les bâtisseurs n’avaient plus besoin de poser
chaque pierre, de câbler chaque serveur : il leur suffisait d’invoquer des services préexistants, comme on fait appel à
des esprits invisibles.

---

## Le Serverless – des sorts sans invocations matérielles

En **2014**, **AWS Lambda** introduisit le concept de **serverless**.  
Plus besoin de maintenir des serveurs : il suffisait de déposer une fonction, et le nuage se chargeait de l’exécuter à
la demande.

Chaque action devenait un **sort jeté dans les nuages** :

- Une requête HTTP déclenche une fonction.
- Un fichier déposé sur un bucket S3 invoque un traitement.
- Un événement dans une base active une réponse automatique.

Cette approche séduisit les bâtisseurs pressés : plus de gestion d’infrastructure, une facturation à l’usage, et une
élasticité quasi infinie.

---

## CI/CD – les rituels automatiques

En parallèle, les pipelines d’intégration et de déploiement continus (**CI/CD**) devinrent les rituels indispensables
des guildes logicielles.

- **Jenkins**, **GitLab CI**, **CircleCI**, **GitHub Actions** : autant d’automates capables de compiler, tester et
  déployer sans intervention humaine.
- Les mises en production devinrent quotidiennes, parfois plusieurs fois par heure, comme des offrandes régulières au
  Cloud.

L’ancienne angoisse du “jour du déploiement” céda la place à une routine fluide, intégrée dans le cycle de
développement.

---

## Les promesses du Cloud

Les magiciens du Cloud offraient de nombreux avantages :

- **Élasticité** : ajouter ou retirer des ressources à la volée.
- **Rapidité** : créer une base de données, un cluster Kubernetes ou un load balancer en quelques clics.
- **Accessibilité** : un coût d’entrée réduit, permettant à des start-ups de rivaliser avec des géants.
- **Écosystèmes complets** : du stockage (S3, Azure Blob) aux bases managées (DynamoDB, BigQuery) en passant par les
  services d’IA (SageMaker, TensorFlow Cloud).

Comme des bibliothèques de grimoires, les catalogues AWS, Azure et GCP grandissaient de mois en mois, couvrant tous les
besoins imaginables.

---

## Les dangers et les contreparties

Mais la magie du Cloud n’était pas gratuite. Derrière la promesse se cachaient de nouveaux risques :

- **Dépendance aux fournisseurs (vendor lock-in)** : un sort appris chez AWS ne se transpose pas toujours chez Azure ou
  GCP.
- **Frais imprévisibles** : une mauvaise configuration pouvait faire exploser la facture en une nuit.
- **Sécurité et confidentialité** : confier ses données à des tiers posait des questions de souveraineté numérique.

Beaucoup d’entreprises découvrirent, parfois à leurs dépens, que la magie avait un prix caché.

---

## Héritage

Cette ère vit l’émergence de l’**approche Cloud Native** : concevoir des applications directement pensées pour le Cloud,
avec des microservices, des conteneurs, du serverless et des architectures pilotées par événements.

Des fondations comme la **CNCF (Cloud Native Computing Foundation, 2015)** furent créées pour encadrer cet écosystème et
promouvoir des outils open source (Kubernetes, Prometheus, Envoy).

---

## Métaphore finale

Le Cloud transforma les bâtisseurs en **sorciers modernes** : au lieu de tailler la pierre et de poser les briques, ils
apprirent à prononcer des incantations qui invoquaient directement des services. Mais chaque sort avait un coût, et
chaque invocation liait un peu plus l’apprenti à son maître.

> La magie du Cloud est puissante, mais elle n’est jamais gratuite.

# PROJET 1 : INVENTAIRE INTRANET PARC INFORMATIQUE

---

## I. Introduction :

Dans le cadre de la gestion d’un parc informatique, il est essentiel pour une organisation de disposer d’une vision précise et centralisée de l’ensemble de ses équipements. Pour répondre à cet enjeu, j’ai mis en place une solution d’inventaire automatisé au sein d’un réseau intranet, permettant de collecter et de remonter les informations matérielles et logicielles des postes utilisateurs vers un serveur centralisé.

Ce projet repose sur l’installation d’un serveur GLPI hébergé en local, ainsi que sur le déploiement de l’agent GLPI sur les postes du réseau. L’utilisation de l’intranet garantit un environnement sécurisé, rapide et totalement maîtrisé, sans dépendance à Internet. L’objectif est d’automatiser l’inventaire, de fiabiliser les données du parc et de faciliter le travail du support informatique grâce à une base d’informations toujours à jour.

Cette solution permet à l’entreprise d’améliorer la maintenance, d’optimiser le suivi du matériel et de renforcer la traçabilité des équipements, tout en s’intégrant parfaitement dans les bonnes pratiques de gestion informatique.

---

## II. Problématique :

Dans un contexte où le parc informatique évolue constamment, l’entreprise doit disposer d’une vision fiable et centralisée de ses équipements pour assurer une maintenance efficace et une gestion optimale des ressources. Or, sans outil d’inventaire automatisé, les informations matérielles et logicielles deviennent rapidement obsolètes, ce qui complique le suivi des postes, augmente les risques d’incidents et ralentit le support technique.
La problématique est donc la suivante : comment mettre en place une solution d’inventaire automatisée, sécurisée et accessible via l’intranet, permettant de collecter et d’actualiser en continu les données du parc informatique ?

---

## III. Objectifs :

La mise en place d’un inventaire automatisé en intranet poursuit plusieurs objectifs essentiels pour la gestion du parc informatique :

1. Centraliser l’ensemble des informations du parc
Rassembler dans une base unique toutes les données matérielles et logicielles des postes de travail afin de disposer d’une vision globale, fiable et constamment à jour.

2. Automatiser la collecte des inventaires
Éliminer les relevés manuels, sources d’erreurs et de perte de temps, en déployant un agent capable d’envoyer automatiquement les informations vers le serveur GLPI.

3. Améliorer la maintenance et le support
Faciliter le diagnostic des incidents, anticiper les pannes et optimiser les interventions grâce à des fiches machines complètes et actualisées.

4. Renforcer la traçabilité et le suivi du matériel
Assurer un suivi précis du cycle de vie des équipements : installation, affectation, mises à jour, remplacement.

5. Sécuriser les échanges en restant dans un environnement intranet
Garantir que toutes les communications entre les agents et le serveur GLPI se font dans un réseau interne maîtrisé, sans exposition à Internet.

6. Optimiser la gestion des licences et des ressources
Identifier les logiciels installés, vérifier leur conformité et mieux planifier les achats ou renouvellements.

---

## IV. Enjeux :

La mise en place d’un inventaire automatisé au sein de l’intranet représente un enjeu stratégique pour la gestion du parc informatique. Elle permet d’améliorer la fiabilité des informations, de renforcer la sécurité du système d’information et d’optimiser les ressources matérielles et logicielles.
L’enjeu principal est de garantir une maîtrise complète du parc informatique, en disposant de données centralisées, actualisées et accessibles uniquement depuis un environnement interne sécurisé.

Sur le plan opérationnel, ce projet vise à réduire les interventions manuelles, limiter les erreurs de saisie et faciliter le travail des équipes techniques grâce à une meilleure visibilité sur l’état des équipements.
Sur le plan organisationnel, il contribue à optimiser les coûts, à anticiper les besoins de renouvellement et à assurer la conformité des logiciels installés.
Enfin, sur le plan sécuritaire, l’utilisation de l’intranet permet de protéger les échanges de données sensibles, en évitant toute exposition du serveur GLPI sur Internet.

---

## V. Contexte :

L’entreprise dispose d’un parc informatique composé de plusieurs postes de travail, périphériques et logiciels utilisés quotidiennement par les collaborateurs. Jusqu’à présent, la gestion de ces équipements reposait sur des relevés manuels ou des informations partielles, ce qui rendait difficile le suivi précis du matériel, l’identification des configurations installées et la planification des opérations de maintenance.

Dans ce contexte, la direction informatique souhaite moderniser et fiabiliser la gestion du parc en mettant en place une solution d’inventaire automatisée, accessible uniquement via l’intranet de l’organisation. Le choix s’est porté sur GLPI, une plateforme open source de gestion de parc et de support, installée localement sur un serveur interne. Pour compléter cette solution, l’agent GLPI est déployé sur les postes du réseau afin de remonter automatiquement les informations matérielles et logicielles.

Ce projet s’inscrit dans une démarche d’amélioration continue du système d’information, avec pour objectif de renforcer la visibilité sur les équipements, d’optimiser les interventions techniques et de garantir une meilleure maîtrise des ressources informatiques

---

## VI. Méthodologie :

La réalisation de ce projet d’inventaire intranet s’est appuyée sur une démarche structurée en plusieurs étapes, permettant d’assurer une mise en place progressive, fiable et conforme aux besoins de l’organisation.

1. Analyse des besoins et définition du périmètre
La première étape a consisté à identifier les équipements concernés par l’inventaire (postes de travail, périphériques, logiciels) ainsi que les attentes du service informatique en matière de centralisation, de mise à jour et de sécurité des données. Cette phase a permis de définir le périmètre fonctionnel et technique du projet.

2. Installation et configuration du serveur GLPI
Un serveur GLPI a été déployé sur l’intranet via WampServer, incluant Apache, PHP et Maria DB. L’environnement a été configuré pour accueillir les inventaires, avec la création de la base de données, l’installation de GLPI et la vérification des modules PHP nécessaires.

3. Mise en place de l’inventaire natif
GLPI 10 intégrant nativement le module d’inventaire, la configuration du serveur a consisté à activer les options d’inventaire, vérifier les droits d’accès et préparer l’URL d’inventaire destinée aux agents.

4. Déploiement de l’agent GLPI sur les postes
L’agent GLPI a été installé sur les postes du réseau intranet. Lors de l’installation, l’URL d’inventaire du serveur GLPI a été renseignée afin de permettre la remontée automatique des informations. Des tests ont été réalisés pour valider la communication entre les agents et le serveur.

5. Tests de remontée et validation des inventaires
Des inventaires manuels ont été déclenchés pour vérifier la bonne transmission des données. Les fiches machines générées dans GLPI ont été analysées afin de contrôler la qualité et l’exhaustivité des informations collectées.

6. Documentation et mise en production
Une documentation technique a été rédigée pour décrire les étapes d’installation, de configuration et de maintenance. Une fois les tests validés, la solution a été déployée en production sur l’ensemble du parc concerné.

---

## VII. Déroulement :

Le projet d’inventaire intranet s’est déroulé en plusieurs phases successives, permettant une mise en place progressive, testée et maîtrisée de la solution. Chaque étape a été réalisée de manière méthodique afin d’assurer la fiabilité du système et la cohérence des données collectées.

1. Préparation de l’environnement technique
La première étape a consisté à installer et configurer l’environnement serveur nécessaire au fonctionnement de GLPI. WampServer a été déployé sur une machine du réseau intranet afin de fournir les services Apache, PHP et Maria DB. Une base de données dédiée a été créée, puis GLPI a été installé et initialisé.

2. Configuration de GLPI et activation de l’inventaire
Une fois GLPI opérationnel, les paramètres essentiels ont été configurés : création des comptes administratifs, définition des entités, vérification des modules PHP requis et activation de l’inventaire natif intégré à GLPI 10. L’URL d’inventaire a été identifiée et testée pour préparer la communication avec les agents.

3. Installation et paramétrage de l’agent GLPI sur les postes
L’agent GLPI a été téléchargé puis installé sur les postes du réseau intranet. Lors de l’installation, l’URL d’inventaire du serveur GLPI a été renseignée afin de permettre la remontée automatique des informations. Des tests ont été réalisés pour valider la bonne communication entre les agents et le serveur.

4. Tests de remontée et validation des données
Des inventaires manuels ont été déclenchés depuis les postes afin de vérifier la transmission correcte des informations. Les fiches machines générées dans GLPI ont été analysées pour contrôler la cohérence des données matérielles et logicielles. Les éventuels ajustements de configuration ont été effectués à cette étape.

5. Documentation et finalisation
Une documentation complète a été rédigée pour décrire l’installation, la configuration et l’utilisation de la solution. Une fois les tests validés, le système a été considéré comme opérationnel et prêt à être utilisé pour la gestion quotidienne du parc informatique.







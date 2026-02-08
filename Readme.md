## PROJET 1 : INVENTAIRE INTRANET PARC INFORMATIQUE

---

## I. Introduction 

Dans le cadre de la gestion d’un parc informatique, il est essentiel pour une organisation de disposer d’une vision précise et centralisée de l’ensemble de ses équipements. Pour répondre à cet enjeu, j’ai mis en place une solution d’inventaire automatisé au sein d’un réseau intranet, permettant de collecter et de remonter les informations matérielles et logicielles d'un poste utilisateur vers un serveur centralisé.

Ce projet repose sur l’installation d’un serveur GLPI hébergé en local, ainsi que sur le déploiement de l’agent GLPI sur le poste du réseau. L’utilisation de l’intranet garantit un environnement sécurisé, rapide et totalement maîtrisé, sans dépendance à Internet. L’objectif est d’automatiser l’inventaire, de fiabiliser les données du parc et de faciliter le travail du support informatique grâce à une base d’informations toujours à jour.

Cette solution permet à l’entreprise d’améliorer la maintenance, d’optimiser le suivi du matériel et de renforcer la traçabilité des équipements, tout en s’intégrant parfaitement dans les bonnes pratiques de gestion informatique.

---

## II. Problématique 

Dans un contexte où le parc informatique évolue constamment, l’entreprise doit disposer d’une vision fiable et centralisée de ses équipements pour assurer une maintenance efficace et une gestion optimale des ressources. Or, sans outil d’inventaire automatisé, les informations matérielles et logicielles deviennent rapidement obsolètes, ce qui complique le suivi des postes, augmente les risques d’incidents et ralentit le support technique.
La problématique est donc la suivante : comment mettre en place une solution d’inventaire automatisée, sécurisée et accessible via l’intranet, permettant de collecter et d’actualiser en continu les données du parc informatique ?

---

## III. Objectifs 

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

## IV. Enjeux 

La mise en place d’un inventaire automatisé au sein de l’intranet représente un enjeu stratégique pour la gestion du parc informatique. Elle permet d’améliorer la fiabilité des informations, de renforcer la sécurité du système d’information et d’optimiser les ressources matérielles et logicielles.
L’enjeu principal est de garantir une maîtrise complète du parc informatique, en disposant de données centralisées, actualisées et accessibles uniquement depuis un environnement interne sécurisé.

Sur le plan opérationnel, ce projet vise à réduire les interventions manuelles, limiter les erreurs de saisie et faciliter le travail des équipes techniques grâce à une meilleure visibilité sur l’état des équipements.
Sur le plan organisationnel, il contribue à optimiser les coûts, à anticiper les besoins de renouvellement et à assurer la conformité des logiciels installés.
Enfin, sur le plan sécuritaire, l’utilisation de l’intranet permet de protéger les échanges de données sensibles, en évitant toute exposition du serveur GLPI sur Internet.

---

## V. Déroulement du projet 

La préparation de l'environnement technique s’est déroulé en plusieurs phases successives, chacune définie dans un cahier des charges initial. Ce document a permis de structurer les actions à mener, d’assurer une progression maîtrisée et de garantir la cohérence de l’ensemble du système mis en place.

### Adressage :

| Machine      | Nommage    |       Adresse IPv4         |   Masque de sous-réseau     |    Serveur DNS     |
|--------------|------------|----------------------------|-----------------------------|--------------------|
| VirtualBox   | PC         |       10.0.0.30            |     255.255.255.0           |     8.8.8.8        |

### Cahier de charge :

1. Installation du système
- Installation de Windows,
- Activation de Windows,
- Installation des mises à jours.

2. Sécurité
- Installation et configuration d'un antivirus,
- Vérification de l'intégrité du système,
- Activation du Pare-feu Windows.

3. Configuration du poste
- Changement du nom du PC,
- Paramétrage du compte utilisateur,
- Configuration réseau,
- Installation des logiciels essentiels.

4. Maintenance et Diagnostic
- Diagnostic complet du matériel,
- Vérification du stockage, RAM, température, état SMART du disque
- Rapport final d'intervention.

---

## VI. Résolution

### 1. Installation du système

### Installation de Windows 10 Entreprise

<p align="center">

<img src="install_PC/01.png" width="400">

<img src="install_PC/02.png" width="400">

<img src="install_PC/03.png" width="400">

<img src="install_PC/04.png" width="400">

<img src="install_PC/05.png" width="400">

<img src="install_PC/06.png" width="400">

<img src="install_PC/07.png" width="400">

<img src="install_PC/08.png" width="400">

<img src="install_PC/09.png" width="400">

<img src="install_PC/10.png" width="400">

<img src="install_PC/11.png" width="400">

<img src="install_PC/12.png" width="400">

</p>

### Activation de Windows 10

Dans la réalisation de ce projet, nous n'avons pas prévu activer Windows. Le poste fonctionne avec quelques limitations serte, mais le système reste utilisable pour installer GLPI, WampServer, l'agent GLPI, etc.

<p align="center">

<img src="activation/01.png" width="400">

</p>

### Installation des mises à jour

L'iso Windows installé sur le poste est récent de version 21H2, il contient déjà des correctifs, des versions .NET, des composants système mis à jour. Donc après installation, Windows peut afficher les mises à jour prête à être appliquée sans avoir besoin d'internet.

<p align="center">

<img src="mises_à_jour/01.png" width="400">

<img src="mises_à_jour/02.png" width="400">

</p>

## 2. Sécurité

### Installation et configuration d'un antivirus

Nous avons prévu installer Avast sur le poste. C'est un antivirus gratuit utilisé en France, offrant une protection en temps réel contre les virus, malwares, phishing et arnaques en ligne. 

<p align="center">

<img src="antivirus/01.png" width="400">

<img src="antivirus/02.png" width="400">

<img src="antivirus/03.png" width="400">

<img src="antivirus/04.png" width="400">

<img src="antivirus/05.png" width="400">

<img src="antivirus/06.png" width="400">

</p>

### Vérification de l'intégrité du système

### Vérification de l'intégrité du système Windows

<p align="center">

<img src="integrite_windows/01.png" width="400">

<img src="integrite_windows/02.png" width="400">

</p>

### Vérification de l'intégrité du magasin de composants (DISM)

<p align="center">

<img src="integrite_magasin/01.png" width="400">

</p>

### Activation du pare-feu Windows




### 5. Diagnostic de tous problèmes matériels

Pour la réalisation du diagnostic, nous avons utilisé PerfMon. Il permet d’analyser en profondeur : l’utilisation du CPU, la consommation de RAM, l’activité du disque, les performances du réseau, les processus gourmands, les goulots d’étranglement du système.

<p align="center">

<img src="diagnostic/01.png" width="400">

<img src="diagnostic/02.png" width="400">

<img src="diagnostic/03.png" width="400">

<img src="diagnostic/04.png" width="400">

<img src="diagnostic/05.png" width="400">

<img src="diagnostic/06.png" width="400">

<img src="diagnostic/07.png" width="400">

<img src="diagnostic/08.png" width="400">

<img src="diagnostic/09.png" width="400">

<img src="diagnostic/10.png" width="400">

<img src="diagnostic/11.png" width="400">

</p>

### 6. Installation WampServer (Serveur GLPI) 

<p align="center">

<img src="serveur_GLPI/01.png" width="400">

<img src="serveur_GLPI/02.png" width="400">

<img src="serveur_GLPI/03.png" width="400">

<img src="serveur_GLPI/04.png" width="400">

<img src="serveur_GLPI/05.png" width="400">

<img src="serveur_GLPI/06.png" width="400">

<img src="serveur_GLPI/07.png" width="400">

<img src="serveur_GLPI/08.png" width="400">

<img src="serveur_GLPI/09.png" width="400">

<img src="serveur_GLPI/10.png" width="400">

</p>

### 7. Configuration GLPI et activation de l’inventaire

<p align="center">

<img src="GLPI/01.png" width="400">

<img src="GLPI/02.png" width="400">

<img src="GLPI/03.png" width="400">

<img src="GLPI/04.png" width="400">

<img src="GLPI/05.png" width="400">

<img src="GLPI/06.png" width="400">

<img src="GLPI/07.png" width="400">

<img src="GLPI/08.png" width="400">

<img src="GLPI/09.png" width="400">

<img src="GLPI/10.png" width="400">

<img src="GLPI/11.png" width="400">

<img src="GLPI/12.png" width="400">

<img src="GLPI/13.png" width="400">

<img src="GLPI/14.png" width="400">

<img src="GLPI/15.png" width="400">

<img src="GLPI/16.png" width="400">

<img src="GLPI/17.png" width="400">

<img src="GLPI/18.png" width="400">

<img src="GLPI/19.png" width="400">

<img src="GLPI/20.png" width="400">

</p>

### 8. Installation de l'agent GLPI

<p align="center">

<img src="agent_GLPI/01.png" width="400">

<img src="agent_GLPI/02.png" width="400">

<img src="agent_GLPI/03.png" width="400">

<img src="agent_GLPI/04.png" width="400">

<img src="agent_GLPI/05.png" width="400">

<img src="agent_GLPI/06.png" width="400">

<img src="agent_GLPI/07.png" width="400">

<img src="agent_GLPI/08.png" width="400">

</p>

### 9. Tests de remontée et validation des données


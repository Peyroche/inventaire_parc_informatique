## PROJET 1 : INVENTAIRE DU PARC INFORMATIQUE

---

## I. Introduction 

<p>Dans le cadre de la gestion d’un parc informatique, il est essentiel pour une organisation de disposer d’une vision précise et centralisée de l’ensemble de ses équipements. Pour répondre à cet enjeu, j’ai mis en place une solution d’inventaire automatisé au sein d’un réseau intranet, permettant de collecter et de remonter les informations matérielles et logicielles d'un poste utilisateur vers un serveur centralisé.</p>

<p>Ce projet repose sur l’installation d’un serveur GLPI hébergé en local, ainsi que sur le déploiement de l’agent GLPI sur le poste du réseau. L’utilisation de l’intranet garantit un environnement sécurisé, rapide et totalement maîtrisé, sans dépendance à Internet. L’objectif est d’automatiser l’inventaire, de fiabiliser les données du parc et de faciliter le travail du support informatique grâce à une base d’informations toujours à jour.</p>

<p>Cette solution permet à l’entreprise d’améliorer la maintenance, d’optimiser le suivi du matériel et de renforcer la traçabilité des équipements, tout en s’intégrant parfaitement dans les bonnes pratiques de gestion informatique.</p>

---

## II. Problématique 

<p>Dans un contexte où le parc informatique évolue constamment, l’entreprise doit disposer d’une vision fiable et centralisée de ses équipements pour assurer une maintenance efficace et une gestion optimale des ressources. Or, sans outil d’inventaire automatisé, les informations matérielles et logicielles deviennent rapidement obsolètes, ce qui complique le suivi des postes, augmente les risques d’incidents et ralentit le support technique.</p>

<p>La problématique est donc la suivante : comment mettre en place une solution d’inventaire automatisée, sécurisée et accessible via l’intranet, permettant de collecter et d’actualiser en continu les données du parc informatique ?</p>

---

## III. Objectifs du projet

<p>La mise en place d’un inventaire automatisé en intranet poursuit plusieurs objectifs essentiels pour la gestion du parc informatique :</p>

<p><b>1. Centraliser l’ensemble des informations du parc :</b></p>
<p>Rassembler dans une base unique toutes les données matérielles et logicielles des postes de travail afin de disposer d’une vision globale, fiable et constamment à jour.</p>

<p><b>2. Automatiser la collecte des inventaires :</b></p>
<p>Éliminer les relevés manuels, sources d’erreurs et de perte de temps, en déployant un agent capable d’envoyer automatiquement les informations vers le serveur GLPI.</p>

<p><b>3. Améliorer la maintenance et le support :</b></p>
<p>Faciliter le diagnostic des incidents, anticiper les pannes et optimiser les interventions grâce à des fiches machines complètes et actualisées.</p>

<p><b>4. Renforcer la traçabilité et le suivi du matériel :</b></p>
<p>Assurer un suivi précis du cycle de vie des équipements : installation, affectation, mises à jour, remplacement.</p>

<p><b>5. Sécuriser les échanges en restant dans un environnement intranet :</b></p>
<p>Garantir que toutes les communications entre les agents et le serveur GLPI se font dans un réseau interne maîtrisé, sans exposition à Internet.</p>

<p><b>6. Optimiser la gestion des licences et des ressources :</b></p>
<p>Identifier les logiciels installés, vérifier leur conformité et mieux planifier les achats ou renouvellements.</p>

---

## IV. Enjeux du projet

<p>La mise en place d’un inventaire automatisé au sein de l’intranet représente un enjeu stratégique pour la gestion du parc informatique. Elle permet d’améliorer la fiabilité des informations, de renforcer la sécurité du système d’information et d’optimiser les ressources matérielles et logicielles.</p>
<p>L’enjeu principal est de garantir une maîtrise complète du parc informatique, en disposant de données centralisées, actualisées et accessibles uniquement depuis un environnement interne sécurisé.</p>

<p>Sur le plan opérationnel, ce projet vise à réduire les interventions manuelles, limiter les erreurs de saisie et faciliter le travail des équipes techniques grâce à une meilleure visibilité sur l’état des équipements.</p>
<p>Sur le plan organisationnel, il contribue à optimiser les coûts, à anticiper les besoins de renouvellement et à assurer la conformité des logiciels installés.</p>
<p>Enfin, sur le plan sécuritaire, l’utilisation de l’intranet permet de protéger les échanges de données sensibles, en évitant toute exposition du serveur GLPI sur Internet.</p>

---

## V. Procédure de déroulement du projet

Ce document a permis de structurer les actions à mener pour une gestion informatique efficace.

<p><b>1. Installation du système</b></p>

<al>
   <li>Installation de Windows</li>
   <li>Activation de Windows</li>
   <li>Installation des mises à jours.</li>
</al>

<p><b>2. Sécurité</b></p>

<al>
   <li>Installation et configuration d'un antivirus</li>
   <li>Vérification de l'intégrité du système</li>
   <li>Activation du Pare-feu Windows.</li>
</al>

<p><b>3. Configuration du poste</b></p>

<al>
   <li>Changement du nom du poste</li>
   <li>Configuration réseau</li>
   <li>Installation des logiciels essentiels.</li>
</al>

<p><b>4. Maintenance et Diagnostic</b></p>

<al>
   <li>Diagnostic complet du matériel</li>
   <li>Vérification du Stockage, RAM, Service Windows, erreurs systèmes</li>
   <li>Rapport final d'intervention.</li>
</al>

---

## VI. Réalisation

### 1. Installation du système

### Installation de Windows 10 Entreprise

<p align="center">

<img src="install_windows/01.png" width="400">

<img src="install_windows/02.png" width="400">

<img src="install_windows/03.png" width="400">

<img src="install_windows/04.png" width="400">

<img src="install_windows/05.png" width="400">

<img src="install_windows/06.png" width="400">

<img src="install_windows/07.png" width="400">

<img src="install_windows/08.png" width="400">

<img src="install_windows/09.png" width="400">

<img src="install_windows/10.png" width="400">

<img src="install_windows/11.png" width="400">

<img src="install_windows/12.png" width="400">

</p>

### Activation de Windows 10

Dans la réalisation de ce projet, nous n'avons pas prévu activer Windows. Le poste fonctionne avec quelques limitations serte, mais le système reste utilisable pour installer GLPI, WampServer, l'agent GLPI, etc.

<p align="center">

<img src="activation_windows/01.png" width="400">

</p>

### Installation des mises à jour

L'iso Windows installé sur le poste est récent de version 21H2, il contient déjà des correctifs, des versions .NET, des composants système mis à jour. Donc après installation, Windows peut afficher les mises à jour prête à être appliquée sans avoir besoin d'internet.

<p align="center">

<img src="mises_à_jour/01.png" width="400">

</p>

### 2. Sécurité

### Installation et configuration d'un antivirus

Nous avons prévu installer Avast sur le poste. C'est un antivirus gratuit utilisé en France, offrant une protection en temps réel contre les virus, malwares, phishing et arnaques en ligne. 

<p align="center">

<img src="antivirus_avast/01.png" width="400">

<img src="antivirus_avast/02.png" width="400">

<img src="antivirus_avast/03.png" width="400">

<img src="antivirus_avast/04.png" width="400">

<img src="antivirus_avast/05.png" width="400">

<img src="antivirus_avast/06.png" width="400">

<img src="antivirus_avast/07.png" width="400">

<img src="antivirus_avast/08.png" width="400">

<img src="antivirus_avast/09.png" width="400">

<img src="antivirus_avast/10.png" width="400">

<img src="antivirus_avast/11.png" width="400">

<img src="antivirus_avast/12.png" width="400">

</p>

### Vérification de l'intégrité du système
L'intégrité consiste à démontrer que les données et fichiers n'ont pas été modifiées, alertés, corrompu ou compromis.

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

<p align="center">

<img src="pare_feu/01.png" width="400">

</p>

### 3. Configuration du poste

### Changement de nom du Poste

<p align="center">

<img src="config_PC01/01.png" width="400">

<img src="config_PC01/02.png" width="400">

<img src="config_PC01/03.png" width="400">

<img src="config_PC01/04.png" width="400">

<img src="config_PC01/05.png" width="400">

<img src="config_PC01/06.png" width="400">

<img src="config_PC01/07.png" width="400">

<img src="config_PC01/08.png" width="400">

<img src="config_PC01/09.png" width="400">

</p>

### Configuration réseau

<p align="center">

<img src="reseau_PC01/01.png" width="400">

<img src="reseau_PC01/02.png" width="400">

<img src="reseau_PC01/03.png" width="400">

<img src="reseau_PC01/04.png" width="400">

<img src="reseau_PC01/05.png" width="400">

<img src="reseau_PC01/06.png" width="400">

</p>

### Installation WampServer (Serveur GLPI) 

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

### Configuration GLPI et activation de l’inventaire

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

</p>

### Installation de l'agent GLPI

<p align="center">

<img src="agent_GLPI/01.png" width="400">

<img src="agent_GLPI/02.png" width="400">

<img src="agent_GLPI/03.png" width="400">

<img src="agent_GLPI/04.png" width="400">

<img src="agent_GLPI/05.png" width="400">

<img src="agent_GLPI/06.png" width="400">

<img src="agent_GLPI/07.png" width="400">

<img src="agent_GLPI/08.png" width="400">

<img src="agent_GLPI/09.png" width="400">

<img src="agent_GLPI/10.png" width="400">

</p>

### Automatisation de l'inventaire

<p align="center">

<img src="automatisation/01.png" width="400">

<img src="automatisation/02.png" width="400">

<img src="automatisation/03.png" width="400">

<img src="automatisation/04.png" width="400">

<img src="automatisation/05.png" width="400">

</p>

### 4. Maintenance et Diagnostic

### Diagnostic de tous problèmes matériels

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

### Vérification du stockage

<p align="center">

<img src="stockage/01.png" width="400">

</p>

### Vérification de la RAM Total

<p align="center">

<img src="RAM_total/01.png" width="400">

</p>

### Vérification de la RAM Libre

<p align="center">

<img src="RAM_libre/01.png" width="400">

</p>

### Vérification des services Windows important

<p align="center">

<img src="service_windows/01.png" width="400">

</p>

### Vérification des 20 dernières erreurs du système

<p align="center">

<img src="20_erreurs/01.png" width="400">

</p>

### Rapport final d'intervention

| Éléments vérifiés     | Résultat obtenu                  | État      | Commentaire                                                                    |  
|-----------------------|----------------------------------|-----------|--------------------------------------------------------------------------------|
| RAM                   | 2 Go total / 581 Mo libres       | Limite    | La RAM disponible représente ~28 %. Fonctionnement correct mais marge réduite  |   
| Stockage              | 53 Go total / 26 Go libres       | Suffisant | Aucun signe de saturation. Espace libre > 25 %.                                |
| Services Windows      | Tous Running sauf Windows Update | Normal    | Windows Update arrêté = comportement normal hors mise à jour.                  | 
| Erreurs système       | Aucune erreur Disk/Ntfs/StorPort | Sain      | Erreurs DCOM/WSearch non critiques, typiques d’une VM.                         |
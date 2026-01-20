# PROJET 1 : INVENTAIRE PARC INFORMATIQUE

---

## I. Contexte :

Dans le cadre d’un projet réalisé sur un réseau virtuel, l’organisation ne dispose d’aucun inventaire structuré. Les équipements sont dispersés et les informations ne sont ni centralisées ni mises à jour. Cette situation rend nécessaire la mise en place d’une démarche professionnelle visant à optimiser la gestion des ressources.

---

## II. Objectifs du projet :

Le projet a pour objectifs :

- d’établir un inventaire structuré,

- d'établir un suivi des indicateurs clés de performance,

- de définir et formaliser une politique de sécurité adaptée à l’organisation,

- d’intégrer un outil automatisé de gestion des ressources, tel que GLPI, afin d’optimiser le suivi et la centralisation des informations.

---

## II.1. Inventaire :

## II.1.1. Inventaire Hardware :

L'inventaire Hardware consiste à collecter les données matériels.

| Equipements | Marque  | N° série | Processeur | RAM  | Stockage | Date d'achat | Fin de Garantie | Localisation |
|-------------|---------|----------|------------|------|----------|--------------|-----------------|--------------|
| Ordinateur  | Acer    |    /     | i5-1235U   | 2 Go | 49,4 Go  | 31/12/2023   |   31/12/2026    | Bureau 1     |
| Ordinateur  | Dell    |    /     | i5-1235U   | 2 Go | 49,4 Go  | 31/12/2024   |   31/12/2027    | Bureau 1     |
| Ordinateur  | Lenovo  |    /     | i5-1235U   | 2 Go | 49,4 Go  | 31/12/2024   |   31/12/2027    | Bureau 2     |
| Serveur     | Dell    |    /     | i5-1235U   | 2 Go | 49,4 Go  | 31/12/2024   |   31/12/2027    | Bureau 2     |


<p align="center">

<img src="configuration/01.png" width="400">

<img src="configuration/02.png" width="400">

</p>


## II.1.2. Inventaire Software :

L'inventaire Software consiste à collecter les données logiciels.

| Logiciel                                    |    Licence      | Numéro licence | Utilisateur autorisé | Version  | Date d'expiration | Date de fin de support |                                                            
|---------------------------------------------|-----------------|----------------|----------------------|----------|-------------------|------------------------|
| Systèmes       | Windows pro 10             |        /        |        /       |        20            |  21H2    |         /         |      13/01/2032        |
| Applicatifs    | Suite Office               |  Microsoft 365  |        /       |        20            |    /     |    31/12/2026     |          /             |
| Utilitaires    | Duplicati                  |  Open source    |        /       |         2            |    /     |         /         |          /             |
| Développements | Visual Studio code         |  Open source    |        /       |         5            |    /     |         /         |          /             |
| Métiers        | CRM                        |        /        |        /       |        10            |    /     |         /         |          /             |
| Serveurs       | Windows server 22          |        /        |        /       |         2            |  21H2    |         /         |      13/01/2032        |


<p align="center">

<img src="version/01.png" width="400">

<img src="version/02.png" width="400">

</p>

---

## II.2. Suivi des indicateurs clés de performance :

Un ensemble de collecteurs de données permet d’enregistrer automatiquement les performances d’un poste ou d’un serveur sur une période définie. Grâce à PerfMon, il est possible de créer un suivi personnalisé des indicateurs clés (CPU, mémoire, disque, réseau) et de planifier exécution. Les données collectées peuvent ensuite être analysées pour anticiper les dégradations et proposer des actions de maintenance préventive.


### Créer un suivi :


<p align="center">

<img src="perfmon/01.png" width="400">

<img src="perfmon/02.png" width="400">

<img src="perfmon/03.png" width="400">

<img src="perfmon/04.png" width="400">

<img src="perfmon/05.png" width="400">

<img src="perfmon/06.png" width="400">

<img src="perfmon/07.png" width="400">

<img src="perfmon/08.png" width="400">

<img src="perfmon/09.png" width="400">

<img src="perfmon/10.png" width="400">

<img src="perfmon/11.png" width="400">

<img src="perfmon/12.png" width="400">

</p>


### Planifier l’exécution :


<p align="center">

<img src="perfmon/13.png" width="400">

<img src="perfmon/14.png" width="400">

<img src="perfmon/15.png" width="400">

<img src="perfmon/16.png" width="400">

<img src="perfmon/17.png" width="400">

<img src="perfmon/18.png" width="400">

</p>
 
---

## II.3. Politique de sécurité :

La Politique de Sécurité des Systèmes d’Information (PSSI) définit les règles permettant d’assurer la confidentialité, l’intégrité et la disponibilité des données et services informatiques de l’organisation MDF.


## Principes généraux :

- La sécurité est l’affaire de tous les utilisateurs.

- Toute action doit respecter les lois en vigueur (RGPD, propriété intellectuelle).

- Les accès sont attribués selon le principe du moindre privilège.

- Les données sensibles doivent être protégées contre toute divulgation non autorisée.


## Gestion des comptes et habilitations :

- Chaque utilisateur dispose d’un compte nominatif.

- Les droits sont attribués via le modèle AGDLP.

- Les comptes administrateurs sont strictement réservés au personnel IT.

- Les comptes inactifs sont désactivés après 30 jours.


## Gestion des mots de passe :

- Longueur minimale : 12 caractères.

- Complexité obligatoire (majuscules, minuscules, chiffres, caractères spéciaux).

- Renouvellement tous les 90 jours.

- Interdiction de partager un mot de passe.


## Sauvegardes :

- Sauvegarde quotidienne des serveurs critiques.

- Conservation 30 jours.

- Tests de restauration trimestriels.


## Postes de travail :

- Verrouillage automatique après 10 minutes.

- Installation de logiciels interdite sans validation IT.

- Antivirus obligatoire.


## Réseau :

- Segmentation par VLAN.

- Filtrage via firewall Fortinet.

- Wi‑Fi invité isolé du réseau interne.






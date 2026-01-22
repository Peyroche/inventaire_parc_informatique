# PROJET 1 : INVENTAIRE PARC INFORMATIQUE

---

## I. Contexte :

Dans le cadre d’un projet réalisé pour une entreprise du nom de MDF sur un réseau virtuel, l’organisation ne dispose d’aucun inventaire structuré. Les équipements sont dispersés et les informations utilisateurs ne sont ni centralisées ni mises à jour. Cette situation rend nécessaire la mise en place d’une démarche professionnelle visant à optimiser la gestion des ressources de l'entreprise.

---

## II. Objectifs du projet :

Le projet a pour objectifs :

- d’établir un inventaire structuré,

- de réaliser une stratégie de maintenance préventive,

- de définir et formaliser une politique de sécurité adaptée à l’organisation,

- d’intégrer un outil automatisé de gestion des ressources, tel que GLPI, afin d’optimiser le suivi et la centralisation des informations.

---

## II.1. Inventaire :

## II.1.1. Inventaire Hardware :

L'inventaire Hardware consiste à collecter les données matériels.

| Postes  | N°  | Marques | Modèles            | Processeur | RAM  | Stockage | Date acquisition | Fin de Garantie | Localisation | Périphériques   | Services            |
|---------|-----|---------|--------------------|------------|------|----------|------------------|-----------------|--------------|-----------------|---------------------|
| PC fixe | 001 | Dell    | Optiplex 7070      | Intel i5   | 2 Go | 49,4 Go  |   10/01/2024     |   10/01/2027    | Bureau 1     | Souris, Clavier | Direction           |
| Laptop  | 002 | Lenovo  | ThinkPad X1 Carbon | Intel i5   | 2 Go | 49,4 Go  |   10/01/2024     |   10/01/2027    | Bureau 1     | Souris, Clavier | Ressources Humaines |
| PC fixe | 003 | HP      | ProDesk 400 G6     | Intel i5   | 2 Go | 49,4 Go  |   10/01/2024     |   10/01/2027    | Bureau 1     | Souris, Clavier | Markéting           |
| PC fixe | 004 | Dell    | Optiplex 7070      | Intel i5   | 2 Go | 49,4 Go  |   10/01/2024     |   10/01/2027    | Bureau 2     | Souris, Clavier | Commercial          |
| Laptop  | 005 | Lenovo  | ThinkPad X1 Carbon | Intel i5   | 2 Go | 49,4 Go  |   20/02/2024     |   20/02/2027    | Bureau 2     | Souris, Clavier | Production          |
| PC fixe | 006 | HP      | ProDesk 400 G6     | Intel i5   | 2 Go | 49,4 Go  |   20/02/2024     |   20/02/2027    | Bureau 2     | Souris, Clavier | Stagiaire           |
| PC fixe | 007 | Dell    | Optiplex 7070      | Intel i5   | 2 Go | 49,4 Go  |   20/02/2024     |   20/02/2027    | Bureau 3     | Souris, Clavier | Comptabilité        |
| Laptop  | 008 | Lenovo  | ThinkPad X1 Carbon | Intel i5   | 2 Go | 49,4 Go  |   20/02/2024     |   20/02/2027    | Bureau 3     | Souris, Clavier | Informatique        |

<p align="center">

<img src="configuration/01.png" width="400">

<img src="configuration/02.png" width="400">              
                                                                       
</p>                                                                    


## II.1.2. Inventaire Software : 

L'inventaire Software consiste à collecter les données logiciels.

| Types Logiciels|   Logiciels        | Licences        | N° de Licence  | Expiration  |  Version   | Fin de support |
|----------------|--------------------|-----------------|----------------|-------------|------------|----------------|
| Systèmes       | Windows pro 10     |        /        |       /        |      /      |   21H2     |   13/01/2032   |
| Applicatifs    | Suite Office       | Microsoft 365   |       /        | 14/09/2026  |     /      |      /         |
| Utilitaires    | Duplicati          |  Open source    |       /        |     /       |     /      |      /         |
| Développements | Visual Studio code |  Open source    |       /        |     /       |     /      |      /         |
| Métiers        | CRM                |        /        |       /        |     /       |     /      |      /         |
| Serveurs       | Windows server 22  |        /        |       /        |     /       |   21H2     |      /         |


<p align="center">

<img src="version/01.png" width="400">

<img src="version/02.png" width="400">

</p>

---

## II.2. Stratégie de Maintenance préventive :

Une stratégie de maintenance préventive peut être ciblée. Par exemple, si l’objectif est de vérifier la stabilité du système, on peut se concentrer uniquement sur la surveillance. Si l’objectif est de renforcer la sécurité, on peut choisir uniquement l’ajustement (correctifs, mises à jour). Si l’objectif est de vérifier l’état du matériel, on peut se limiter à l’inspection.

Voici un tableau simple pour guider le choix :

|  Objectif                                                                                                                  | Action pertinente |      
|----------------------------------------------------------------------------------------------------------------------------|-------------------|
| Examiner régulièrement l’état physique du matériel informatique, comme les câbles, les ventilateurs, ou les disques durs   | Inspection        |                                                                           
| Suivi des indicateurs clés des performances (température, utilisation CPU, espace disque)                                  | Surveillance      | 
| Réaliser des mises à jour des produits Microsoft, application des correctifs de sécurité, ajustement des paramètres réseau | Ajustement        | 

Dans le cadre de la maintenance préventive, nous avons choisi de réaliser deux actions :
- l’action de surveillance,
- l'action d'ajustement.


## II.2.1. Action de surveillance :

### Création d'un suivi des indicateurs clés des performances CPU/RAM/Stockage via PerfMon :

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


### Planifier l'exécution du suivi :

<p align="center">

<img src="perfmon/13.png" width="400">

<img src="perfmon/14.png" width="400">

<img src="perfmon/15.png" width="400">

<img src="perfmon/16.png" width="400">

<img src="perfmon/17.png" width="400">

<img src="perfmon/18.png" width="400">

</p>
 

## II.2.2. Action d'ajustement

### Réaliser la mise à jour des produits Microsoft via WSUS :







---

## II.4 Mises à jours des configurations matérielles :

Les mises à jour matérielles concernent les composants physiques du parc informatique. Elles sont nécessaires lorsque le matériel devient insuffisant, obsolète ou limite les performances. 

---

## II.4 Politique de sécurité :

La Politique de Sécurité des Systèmes d’Information (PSSI) définit les règles permettant d’assurer la confidentialité, l’intégrité et la disponibilité des données et services informatiques de l’organisation MDF.


### Principes généraux :

- La sécurité est l’affaire de tous les utilisateurs.

- Toute action doit respecter les lois en vigueur (RGPD, propriété intellectuelle).

- Les accès sont attribués selon le principe du moindre privilège.

- Les données sensibles doivent être protégées contre toute divulgation non autorisée.


### Gestion des comptes et habilitations :

- Chaque utilisateur dispose d’un compte nominatif.

- Les droits sont attribués via le modèle AGDLP.

- Les comptes administrateurs sont strictement réservés au personnel IT.

- Les comptes inactifs sont désactivés après 30 jours.


### Gestion des mots de passe :

- Longueur minimale : 12 caractères.

- Complexité obligatoire (majuscules, minuscules, chiffres, caractères spéciaux).

- Renouvellement tous les 90 jours.

- Interdiction de partager un mot de passe.


### Sauvegardes :

- Sauvegarde quotidienne des serveurs critiques.

- Conservation 30 jours.

- Tests de restauration trimestriels.


### Postes de travail :

- Verrouillage automatique après 10 minutes.

- Installation de logiciels interdite sans validation IT.

- Windows Defender Antivirus obligatoire.


### Réseau :

- Segmentation par VLAN.

- Filtrage via firewall Fortinet.

- Wi‑Fi invité isolé du réseau interne.

---

## II.5. Automatisé la gestion avec GLPI :

GLPI est un logiciel libre de gestion informatique (ITSM) qui permet de gérer un parc informatique, les utilisateurs, les tickets d’assistance et l’ensemble des services IT d’une organisation. C’est l’un des outils les plus utilisés en France pour inventorier, suivre et administrer un système d’information.

### II.5.1 Installation de GLPI :





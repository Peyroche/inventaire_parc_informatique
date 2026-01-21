# PROJET 1 : INVENTAIRE PARC INFORMATIQUE

---

## I. Contexte :

Dans le cadre d’un projet réalisé pour une entreprise du nom de MDF sur un réseau virtuel, l’organisation ne dispose d’aucun inventaire structuré. Les équipements sont dispersés et les informations utilisateurs ne sont ni centralisées ni mises à jour. Cette situation rend nécessaire la mise en place d’une démarche professionnelle visant à optimiser la gestion des ressources de l'entreprise.

---

## II. Objectifs du projet :

Le projet a pour objectifs :

- d’établir un inventaire structuré,

- d'établir un suivi des indicateurs clés de performance,

- de réaliser les mises à jours régulières des configurations matérielles et logicielles

- de définir et formaliser une politique de sécurité adaptée à l’organisation,

- d’intégrer un outil automatisé de gestion des ressources, tel que GLPI, afin d’optimiser le suivi et la centralisation des informations.

---

## II.1. Inventaire :

## II.1.1. Inventaire Hardware :

L'inventaire Hardware consiste à collecter les données matériels.

| poste   | N°  | Marques | Modèles            | Processeur | RAM  | Stockage | Date acquisition | Fin de Garantie | Localisation | Périphériques   | Services            |
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

## II.3 Mises à jours des configuration matérielles et logicielles :

Réaliser des mises à jour régulières des configurations matérielles et logicielles est essentiel pour garantir un niveau optimal de sécurité, de stabilité et de performance au sein du système d’information. Cela inclut l’application systématique des correctifs de sécurité, la mise à jour des pilotes, ainsi que l’ajustement des paramètres réseau en fonction des besoins opérationnels. Pour automatiser et centraliser la gestion des mises à jour, l’entreprise peut s’appuyer sur une solution telle que WSUS (Windows Server Update Services), permettant de contrôler, valider et déployer les correctifs sur l’ensemble du parc informatique.

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

II.5. Automatisé la gestion avec GLPI :


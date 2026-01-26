# PROJET 1 : INVENTAIRE PARC INFORMATIQUE

---

## I. Contexte :

Dans le cadre d’un projet réalisé pour une entreprise du nom de MDF sur un réseau virtuel, l’organisation ne dispose d’aucun inventaire structuré. Les équipements sont dispersés et les informations utilisateurs ne sont ni centralisées ni mises à jour. Cette situation rend nécessaire la mise en place d’une démarche professionnelle visant à optimiser la gestion des ressources de l'entreprise.

---

## II. Objectifs du projet :

Le projet a pour objectifs :

- configurer les postes clients et serveurs
- d’établir un inventaire structuré,
- de réaliser un diagnostic du système,
- de définir une politique de sécurité adaptée à l’organisation,
- d’intégrer un outil automatisé GLPI.

---

## II.1. Configuration des postes clients et serveurs :

Avant de faire un inventaire propre et professionnel, il y a toujours une phase de configuration des postes et des serveurs. C’est même une étape essentielle pour que l'inventaire soit clair, cohérent et exploitable.

| N° | Code   | Postes   | Services     |
|----|--------|----------|--------------|
| 1  | SRV    | Fixe     |    /         |
| 2  | PC01   | Fixe     | IT           |  
| 3  | PC02   | Fixe     | Comptabilité |
| 4  | PC03   | Portable | Marketing    |

## Configuration poste client :

<p align="center">

<img src="pc/01.png" width="400"> 
                                                                  
<img src="pc/02.png" width="400">   
                                         
<img src="pc/03.png" width="400">   

<img src="pc/04.png" width="400">   

<img src="pc/05.png" width="400">   

<img src="pc/06.png" width="400">   

<img src="pc/07.png" width="400">   

<img src="pc/08.png" width="400">   

<img src="pc/09.png" width="400">   

<img src="pc/10.png" width="400">   

<img src="pc/11.png" width="400">   

<img src="pc/12.png" width="400">   

<img src="pc/13.png" width="400">   

<img src="pc/14.png" width="400">   

<img src="pc/15.png" width="400">   

<img src="pc/16.png" width="400">   

<img src="pc/17.png" width="400">   

<img src="pc/18.png" width="400">   

<img src="pc/19.png" width="400">   
                   
</p>                                                                    


## Configuration serveur :

<p align="center">

<img src="srv/01.png" width="400"> 
                                                                  
<img src="srv/02.png" width="400">   
                                         
<img src="srv/03.png" width="400">   

<img src="srv/04.png" width="400">   

<img src="srv/05.png" width="400">   

<img src="srv/06.png" width="400">   

<img src="srv/07.png" width="400">   

<img src="srv/08.png" width="400">   

<img src="srv/09.png" width="400">   

<img src="srv/10.png" width="400">   

<img src="srv/11.png" width="400">   

<img src="srv/12.png" width="400">   

<img src="srv/13.png" width="400">   

<img src="srv/14.png" width="400">   

<img src="srv/15.png" width="400">   

<img src="srv/16.png" width="400">   

<img src="srv/17.png" width="400">   

<img src="srv/18.png" width="400">   
                   
</p>                                                                    

---

## II.2. Inventaire :

## II.2.1. Inventaire Hardware :

L'inventaire Hardware consiste à collecter les données matériels.

| N° | Code   | Postes   | Marques        | Modèles    | N° de série                                       | CPU       | RAM  |  GPU   | Stockage | Périphériques   |
|----|--------|----------|----------------|------------|---------------------------------------------------|-----------|------|--------|----------|-----------------|
| 1  | SRV    | Fixe     | innotek GmbH   | VirtuelBox | VirtuelBox-b9835393-e1a5-4857-9b6b-97f2698c9b14   | Intel i5  | 2 Go |   /    |  50 GB   | Souris, Clavier | 
| 2  | PC01   | Fixe     | innotek Gmbh   | VirtuelBox | VirtuelBox-8b199364-B669-49e4-8303-913e1987b5b9   | Intel i5  | 2 Go |   /    |  50 GB   | Souris, Clavier | 
| 3  | PC02   | Portable | innotek GmbH   | VirtuelBox | VirtuelBox-                                       | Intel i5  | 2 Go |   /    |  50 GB   |        /        | 
| 4  | PC03   | Portable | innotek GmbH   | VirtuelBox | VirtuelBox-                                       | Intel i5  | 2 Go |   /    |  50 GB   |        /        | 

<p align="center">

<img src="configuration/01.png" width="400"> 
                                                                  
<img src="configuration/02.png" width="400"> 

<img src="configuration/03.png" width="400">

<img src="configuration/04.png" width="400">
                                                              
</p> 

                                                          
## II.2.2. Inventaire Software : 

L'inventaire Software consiste à collecter les données logiciels.

| Types de Logiciels | Logiciels                     | Licences    | N° de Licence | Expiration | Version | Fin de support |
|--------------------|-------------------------------|-------------|---------------|------------|---------|----------------|
| Systèmes           | Windows pro 10                |      /      |       /       |     /      |   21H2  |   13/01/2032   |
| Applicatifs        | Libre Office                  | Open source |       /       |     /      |     /   |       /        |
| Développements     | Visual Studio code            | Open source |       /       |     /      |     /   |       /        |
| Métiers            | CRM                           |      /      |       /       |     /      |     /   |       /        |
| Serveurs           | Windows server 22, WampServer |      /      |       /       |     /      |   21H2  |   13/01/2032   |


<p align="center">

<img src="version/01.png" width="400">

<img src="version/02.png" width="400">

</p>


## II.2.3. Inventaire Globale : 
 
| N° | Code   | Postes   | Marques      |             Logiciels                           | CPU       | RAM  | GPU | Stockage | Périphériques   | Etats      | Services     | Lieu |
|----|--------|----------|--------------|-------------------------------------------------|-----------|------|-----|----------|-----------------|------------|--------------|------|
| 1  | SRV    | Fixe     | innotek GmbH | Windows server 22                               | Intel i5  | 2 Go |  /  |  50 GB   | Souris, Clavier | En service | /            | B1   |
| 2  | PC01   | Fixe     | innotek GmbH | Windows pro 10, WampServer, Visuel Studio code  | Intel i5  | 2 Go |  /  |  50 GB   | Souris, Clavier | En service | IT           | B1   |
| 4  | PC02   | Portable | innotek GmbH | Windows pro 10, Libre Office, CRM               | Intel i5  | 2 Go |  /  |  50 GB   |        /        | En service | Comptabilité | B2   |
| 5  | PC03   | Portable | innotek GmbH | Windows pro 10, Libre Office, CRM               | Intel i5  | 2 Go |  /  |  50 GB   |        /        | En service | Marketing    | B2   |
                                                                                           
---

## II.3. Diagnostic du système :

## Diagnostic server :

<p align="center">

<img src="diagnostic_srv/01.png" width="400">

<img src="diagnostic_srv/02.png" width="400">

<img src="diagnostic_srv/03.png" width="400">

<img src="diagnostic_srv/04.png" width="400">

<img src="diagnostic_srv/05.png" width="400">

<img src="diagnostic_srv/06.png" width="400">

<img src="diagnostic_srv/07.png" width="400">

<img src="diagnostic_srv/08.png" width="400">

<img src="diagnostic_srv/09.png" width="400">

<img src="diagnostic_srv/10.png" width="400">

<img src="diagnostic_srv/11.png" width="400">

<img src="diagnostic_srv/12.png" width="400">

<img src="diagnostic_srv/13.png" width="400">

<img src="diagnostic_srv/14.png" width="400">

</p>


## Diagnostic poste client :

<p align="center">

<img src="diagnostic_pc/01.png" width="400">

<img src="diagnostic_pc/02.png" width="400">

<img src="diagnostic_pc/03.png" width="400">

<img src="diagnostic_pc/04.png" width="400">

<img src="diagnostic_pc/05.png" width="400">

<img src="diagnostic_pc/06.png" width="400">

<img src="diagnostic_pc/07.png" width="400">

<img src="diagnostic_pc/08.png" width="400">

<img src="diagnostic_pc/09.png" width="400">

<img src="diagnostic_pc/10.png" width="400">

<img src="diagnostic_pc/11.png" width="400">

<img src="diagnostic_pc/12.png" width="400">

<img src="diagnostic_pc/13.png" width="400">

<img src="diagnostic_pc/14.png" width="400">

</p>

Le fait que Windows 10 Enterprise LTSC ne soit pas activé peut indirectement empêcher l’installation automatique de certains pilotes, surtout dans une machine virtuelle. Windows non activé limite certaines fonctionnalités, notamment : personnalisation, accès complet à Windows Update, téléchargement de pilotes facultatifs ou tiers.

Certains périphériques, comme les contrôleurs PCI virtuels, restent non reconnus car Windows ne télécharge pas leur pilote automatiquement.

<p align="center">
<img src="windows/01.png" width="400">
</p>


La solution dans tout ça serait d'activer une clé MAK ou une clé KMS.

Pour rappel une clé MAK est une clé de produit Windows utilisée dans les entreprises pour activer définitivement un certain nombre de machines. 

Fonctionnement : 

- elle active Windows une seule fois par machine, 
- l’activation se fait via Internet directement auprès de Microsoft, 
- une fois activé, le PC reste activé à vie, même hors réseau.

Tandis qu'une clé KMS est une clé utilisée pour activer Windows via un serveur d’activation interne dans une organisation. 

Fonctionnement :

- le PC contacte un serveur KMS interne, 
- l’activation est temporaire : 180 jours, 
- le PC doit renouveler son activation régulièrement en restant sur le réseau de l’entreprise.

---

## II.3. Politique de sécurité :

La Politique de Sécurité des Systèmes d’Information (PSSI) définit les règles permettant d’assurer la confidentialité, l’intégrité et la disponibilité des données et services informatiques de l’organisation.

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

---

## II.4. Automatisation de la gestion avec GLPI :

Prérequis à télécharger :

- WampServer (PHP version 7.4.33) : https://www.wampserver.com
- Packages Microsoft Visual C++ : https://wampserver.aviatechno.net
- GLPI version 10.0.6 : https://www.glpi-project.org/en/new-version-glpi-10-0-6/
- OCS Inventory NG version 2.0.5 : https://github.com/fusioninventory/fusioninventory-for-glpi/releases
- Fusion Inventory Version 10.0.6 + 1.1 : https://github.com/pluginsGLPI/ocsinventoryng/releases/tag/2.0.5

Une fois téléchargé et décompressé, les documents ont été envoyé sur la machine virtuelle.

## Hyperviseur :

<p align="center">
<img src="hyperviseur_1/01.png" width="400">
</p>

## Installation VBoxWindowsAdditions :

VBoxWindowsAdditions (appelée aussi Guest Additions) sert à transformer les fichiers et logiciels dans un environnement virtuel.

<p align="center">
<img src="vbox/01.png" width="400">
<img src="vbox/02.png" width="400">
<img src="vbox/03.png" width="400">
<img src="vbox/04.png" width="400">
<img src="vbox/05.png" width="400">
<img src="vbox/06.png" width="400">
<img src="vbox/07.png" width="400">
</p>


## Hyperviseur :

<p align="center">
<img src="hyperviseur_2/01.png" width="400">
<img src="hyperviseur_2/02.png" width="400">
</p>

## Installation WampServer :

WampServer est une plateforme de développement web pour Windows. Elle permet de créer et tester des sites web en local (sur ton PC), d'utiliser des technologies comme Apache, MySQL, PHP, de gérer tes bases de données avec phpMyAdmin.

<p align="center">
<img src="wampserver/01.png" width="400">
<img src="wampserver/02.png" width="400">
<img src="wampserver/03.png" width="400">
<img src="wampserver/04.png" width="400">
<img src="wampserver/05.png" width="400">
<img src="wampserver/06.png" width="400">
<img src="wampserver/07.png" width="400">
<img src="wampserver/08.png" width="400">
<img src="wampserver/09.png" width="400">
<img src="wampserver/10.png" width="400">
</p>

## Installation GLPI :

GLPI est un logiciel libre de gestion informatique (ITSM) qui permet de gérer un parc informatique, les utilisateurs, les tickets d’assistance et l’ensemble des services IT d’une organisation. GLPI permet d’appliquer concrètement les processus ITIL dans une organisation. 

ITIL (Information Technology Infrastructure Library) est un référentiel international qui décrit les meilleures pratiques pour organiser un service informatique. Il définit des processus tels que : gestion des incidents, gestion des demandes, gestion des problèmes, gestion des changements, gestion des actifs (CMDB), gestion des connaissances, gestion du catalogue de services, suivi des SLA et qualité de service.

<p align="center">
<img src="glpi/01.png" width="400">
<img src="glpi/02.png" width="400">
<img src="glpi/03.png" width="400">
<img src="glpi/04.png" width="400">
<img src="glpi/05.png" width="400">
<img src="glpi/06.png" width="400">
<img src="glpi/07.png" width="400">
<img src="glpi/08.png" width="400">
<img src="glpi/09.png" width="400">
<img src="glpi/10.png" width="400">
<img src="glpi/11.png" width="400">
<img src="glpi/12.png" width="400">
<img src="glpi/13.png" width="400">
<img src="glpi/14.png" width="400">
</p>


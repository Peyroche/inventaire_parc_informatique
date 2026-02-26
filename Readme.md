## Projet 1 : Inventaire du parc informatique d'une pme

---

## I. Introduction 

<p>Dans le cadre de la gestion d’un parc informatique, il est essentiel pour une organisation de disposer d’une vision précise et centralisée de l’ensemble de ses équipements. Pour répondre à cet enjeu, j’ai mis en place une solution d’inventaire automatisé au sein d’un réseau, permettant de collecter et de remonter les informations matérielles et logicielles d'un poste utilisateur vers un serveur centralisé.</p>

<p>Ce projet repose sur l’installation d’un serveur linux (debian) ocs Inventory hébergé en local, ainsi que le déploiement de l’agent ocs sur les postes clients du réseau. L’objectif est d’automatiser l’inventaire, de fiabiliser les données du parc et de faciliter le travail du support informatique grâce à une base d’informations toujours à jour.</p>

<p>Cette solution permet à l’entreprise d’améliorer la maintenance, d’optimiser le suivi du matériel et de renforcer la traçabilité des équipements, tout en s’intégrant parfaitement dans les bonnes pratiques de gestion informatique.</p>

---

## II. Problématique 

<p>Dans un contexte où le parc informatique évolue constamment, l’entreprise doit disposer d’une vision fiable et centralisée de ses équipements pour assurer une maintenance efficace et une gestion optimale des ressources. Or, sans outil d’inventaire automatisé, les informations matérielles et logicielles deviennent rapidement obsolètes, ce qui complique le suivi des postes, augmente les risques d’incidents et ralentit le support technique.</p>

<p>La problématique est donc de savoir : comment mettre en place une solution d’inventaire automatisée permettant de collecter et d’actualiser en continu les données du parc informatique ?</p>

---

## III. Objectifs

<p>La mise en place d’un inventaire automatisé en intranet poursuit plusieurs objectifs essentiels pour la gestion du parc informatique :</p>

<p><b>1. Centraliser l’ensemble des informations du parc</b></p>
<p>Rassembler dans une base unique toutes les données matérielles et logicielles des postes de travail afin de disposer d’une vision globale, fiable et constamment à jour.</p>

<p><b>2. Automatiser la collecte des inventaires</b></p>
<p>Éliminer les relevés manuels, sources d’erreurs et de perte de temps, en déployant un agent capable d’envoyer automatiquement les informations vers le serveur ocs.</p>

<p><b>3. Améliorer la maintenance et le support</b></p>
<p>Faciliter le diagnostic des incidents, anticiper les pannes et optimiser les interventions grâce à des fiches machines complètes et actualisées.</p>

<p><b>4. Renforcer la traçabilité et le suivi du matériel</b></p>
<p>Assurer un suivi précis du cycle de vie des équipements : installation, affectation, mises à jour, remplacement.</p>

<p><b>5. Sécuriser les échanges en restant dans un environnement intranet</b></p>
<p>Garantir que toutes les communications entre les agents et le serveur ocs se font dans un réseau interne maîtrisé, sans exposition à Internet.</p>

<p><b>6. Optimiser la gestion des licences et des ressources</b></p>
<p>Identifier les logiciels installés, vérifier leur conformité et mieux planifier les achats ou renouvellements.</p>

---

## IV. Procédures

<p>Dans le cadre de l’inventaire du parc informatique, une procédure d'intervention a été réalisée :</p>

<p><b>1. Installation système</b></p>
<p>- Installation de Windows 10 Entreprise sur les postes clients</p>
<p>- Activation de Windows 10 Entreprise sur les postes clients</p>
<p>- Installation des mises à jours des postes clients.</p>

<p><b>2. Sécurité</b></p>
<p>- Installation et configuration antivirus sur les postes clients</p>
<p>- Vérification de l'intégrité du système</p>
<p>- Activation pare-feu.</p>

<p><b>3. Configuration des postes</b></p>
<p>- Changement de nom des postes clients</p>
<p>- Configuration réseau.</p>

<p><b>4. Maintenance et Diagnostic</b></p>
<p>- Diagnostic complet du matériel</p>
<p>- Vérification du Stockage, RAM, Service Windows, erreurs systèmes.</p>

<p><b>5. Automatisation de l'inventaire</b></p>
<p>- Installation du server linux (debian)</p>
<p>- Installation ocs inventory</p>
<p>- Installation agent ocs sur les postes clients.</p>

---

## V. Réalisations

### 1. Installation système

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

<img src="install_windows/13.png" width="400">

</p>

### Activation de Windows 10 Entreprise

Dans la réalisation de ce projet, nous n'avons pu activer Windows par manque de clé. Le poste fonctionne avec quelques limitations serte, mais le système reste utilisable pour installer GLPI, WampServer, l'agent GLPI, etc.

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

Avast a été installé sur le poste client. Avast est un antivirus gratuit offrant une protection en temps réel contre les virus, malwares, phishing et arnaques en ligne. 

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

<p>Le programme de protection des ressources Windows n'a trouvé aucune violation d'intégrité.</p>


### Vérification de l'intégrité du magasin de composants (DISM)

<p align="center">

<img src="integrite_magasin/01.png" width="400">

</p>

<p>Aucun endommagement du magasin de composants n'a été détecté. L'opération a donc réussi.</p>

### Activation du pare-feu Windows

<p align="center">

<img src="pare_feu/01.png" width="400">

</p>

<p>Windows ne reconnaît pas le réseau, il applique automatiquement les règles les plus strictes. Activer le pare‑feu dans ce cas est obligatoire pour éviter les risques.</p>

### 3. Configuration du poste client

### Changement de nom du poste client

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

### Configuration réseau du poste client

<p align="center">

<img src="reseau_PC01/01.png" width="400">

<img src="reseau_PC01/02.png" width="400">

<img src="reseau_PC01/03.png" width="400">

<img src="reseau_PC01/04.png" width="400">

<img src="reseau_PC01/05.png" width="400">

<img src="reseau_PC01/06.png" width="400">

</p>

### 4. Maintenance

### Diagnostic du poste client

PerfMon a été utilisé pour diagnostiquer le poste client.

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

<p>Le diagnostic système met en évidence un fonctionnement globalement stable du poste de travail : le processeur, le disque, les pilotes et les services système ne présentent aucune anomalie. En revanche, l’analyse signale une évaluation mémoire très faible, susceptible d’entraîner des ralentissements et une dégradation des performances.</p>

<p>Il est recommandé de réduire le nombre d’applications ouvertes simultanément, de désactiver les programmes inutiles au démarrage et, si les problèmes persistent, d’envisager une mise à niveau de la mémoire RAM.</p>


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

<p>L’analyse initiale signalait une évaluation mémoire médiocre, indiquant que le système était fortement sollicité au moment du diagnostic. Cependant, une vérification ultérieure via PowerShell montre que la machine dispose d’une quantité très importante de mémoire physique libre (plus de 500 Go).</p>

<p>Cela confirme que la dégradation des performances observée n’est pas liée à un manque de RAM, mais à une surcharge temporaire due à des applications ou processus actifs au moment de l’analyse. Le système ne présente donc pas de limitation matérielle, mais un pic d’utilisation ponctuel.</p>

### Vérification des services Windows important

<p align="center">

<img src="service_windows/01.png" width="400">

</p>

### Vérification des 20 dernières erreurs du système

<p align="center">

<img src="20_erreurs/01.png" width="400">

</p>

### 5. Automatisation de l'inventaire

### Installation du serveur linux (debian)

<p align="center">

<img src="debian/01.png" width="400">

<img src="debian/02.png" width="400">

<img src="debian/03.png" width="400">

<img src="debian/04.png" width="400">

<img src="debian/05.png" width="400">

<img src="debian/06.png" width="400">

<img src="debian/07.png" width="400">

<img src="debian/08.png" width="400">

<img src="debian/09.png" width="400">

<img src="debian/10.png" width="400">

<img src="debian/11.png" width="400">

<img src="debian/12.png" width="400">

<img src="debian/13.png" width="400">

<img src="debian/14.png" width="400">

<img src="debian/16.png" width="400">

<img src="debian/17.png" width="400">

<img src="debian/18.png" width="400">

<img src="debian/18.png" width="400">

<img src="debian/19.png" width="400">

<img src="debian/20.png" width="400">

<img src="debian/21.png" width="400">

<img src="debian/22.png" width="400">

<img src="debian/23.png" width="400">

</p>


### Installation de l'agent ocs sur les postes clients

<p align="center">

<img src="agent_ocs/01.png" width="400">

<img src="agent_ocs/02.png" width="400">

<img src="agent_ocs/03.png" width="400">

<img src="agent_ocs/04.png" width="400">

<img src="agent_ocs/05.png" width="400">

<img src="agent_ocs/06.png" width="400">

<img src="agent_ocs/07.png" width="400">

<img src="agent_ocs/08.png" width="400">

<img src="agent_ocs/09.png" width="400">

<img src="agent_ocs/10.png" width="400">

</p>

---

## VI. Conclusion

<p>L’intervention menée dans le cadre de l’inventaire du parc informatique a permis de mettre en place une solution complète, fiable et opérationnelle pour centraliser et automatiser la gestion des équipements informatiques. L’installation du serveur GLPI, du poste client, de l’agent d’inventaire et des différents outils de diagnostic a abouti à un environnement fonctionnel capable de remonter automatiquement les informations matérielles et logicielles du poste vers le serveur intranet.</p>

<p>Les différentes étapes : installation du système, configuration réseau, sécurisation du poste, déploiement de GLPI et de son agent, automatisation de l’inventaire et diagnostics avancés  ont été réalisées avec succès. Les analyses effectuées montrent que le poste ne présente aucune défaillance matérielle : le processeur, le stockage, les pilotes et les services critiques fonctionnent normalement. Les alertes relevées concernent essentiellement des dysfonctionnements logiciels ponctuels, notamment des services (GLPI Agent, Avast) ne démarrant pas correctement ou des arrêts système non propres. Ces anomalies n’affectent pas la stabilité globale du poste et peuvent être corrigées par des ajustements de configuration.</p>

<p>L’évaluation mémoire initialement jugée faible s’explique par une surcharge temporaire lors du diagnostic, comme confirmé par les mesures PowerShell montrant une quantité très importante de RAM disponible. Le système ne souffre donc pas d’un manque de ressources, mais d’un pic d’utilisation ponctuel.</p>

<p>Au final, le projet atteint pleinement ses objectifs : l’inventaire est automatisé, les données sont centralisées et fiabilisées, la maintenance est facilitée, la traçabilité du matériel est renforcée, et l’ensemble fonctionne dans un environnement sécurisé et maîtrisé.</p>
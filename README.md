![HectorLayak — Comprendre. Construire. Faire vivre.](assets/showcase/hero-fr.svg)

<p align="center"><a href="#projets-choisis">Six projets</a> · <a href="#la-carte-de-latelier">La carte</a> · <a href="#tout-latelier">33 projets</a> · <a href="https://floriansola.fr">Site personnel ↗</a> · <a href="README.en.md">English</a></p>

Je construis des plateformes métier, des outils pour les développeurs et des mondes en réseau. Du compilateur à l'interface, je travaille les contrats, l'autorité et la cohérence de l'état.

**C# / .NET · Rust · TypeScript · C / C++**

## Projets choisis

[![AINDEX — Les agents opèrent. Les humains supervisent le projet.](assets/showcase/aindex-fr.svg)](https://floriansola.fr/projects/aindex)

AINDEX organise le travail des agents autour du projet : missions, contexte du dépôt, changements et vérifications. Le moteur Rust porte l’autorité ; le Studio donne aux humains une vue commune pour superviser et décider.

<details>
<summary>Architecture et parcours</summary>

**Une autorité de projet.** Le moteur Rust possède les tâches, les réservations, les validations et leur provenance. Le Studio, l’extension et la passerelle présentent ces contrats ; les interfaces restent alignées sur la même autorité.

**Le contexte arrive au moment utile.** Une capsule rassemble le contrat complet de la mission et une sélection de références courantes. Un adaptateur d’hôte peut la fournir lors des événements de travail ; la lecture aindex_context sert de point d’accès quand un rafraîchissement est nécessaire.

1. Relier un objectif à une mission, à son périmètre et aux règles du dépôt.
2. Fournir à l’agent le contexte utile au moment du travail : contrats, dépendances, références et état observé.
3. Suivre les changements et l’activité dans une supervision humaine commune au Studio et à ses lecteurs.
4. Examiner les vérifications, résoudre les contradictions et prendre la décision d’intégration.

</details>

[Explorer le projet ↗](https://floriansola.fr/projects/aindex)

[![HECTOR — Un langage pour exprimer les comportements, compiler et examiner les contrats.](assets/showcase/hector-fr.svg)](https://floriansola.fr/projects/hector)

HECTOR est un langage et un compilateur natif pour auteurs humains et agents. Types, effets et contrats accompagnent des noyaux métier exécutables en natif et WebAssembly.

<details>
<summary>Architecture et parcours</summary>

**Le compilateur porte la sémantique.** Les unités json, syntax, foundation, core et driver sont écrites en Hector. Le bootstrap reconstruit la chaîne depuis ses seeds ; LLVM assure l’émission native. Les lanceurs dirigent vers cette même autorité.

**Des contrats observables.** Préconditions, postconditions, effets et identités de source accompagnent l’analyse et l’exécution. Les faits du checker alimentent les contrôles de sélection et de compatibilité avec une référence.

1. Écrire un comportement en Hector avec ses types, effets et clauses de contrat.
2. Analyser les sources avec le compilateur natif et examiner les faits produits par le checker.
3. Construire une bibliothèque native ou WebAssembly pour un consommateur externe.
4. Comparer les interfaces et les propriétés de publication, puis qualifier le parcours sur son hôte cible.

</details>

[Explorer le projet ↗](https://floriansola.fr/projects/hector)

[![OneRP — Un socle SaaS pour exploiter des mondes roleplay FiveM.](assets/showcase/onerp-framework-fr.svg)](https://floriansola.fr/projects/onerp-framework)

OneRP associe un backend SaaS, une administration et des modules FiveM. Personnages, économie, inventaires, véhicules, logements et activités partagent des services métier réactifs et des interfaces React en jeu.

<details>
<summary>Architecture et parcours</summary>

**Un état métier réactif.** Fusion relie les lectures à leurs dépendances. Les mutations invalident les données concernées ; les sentinelles propres au joueur limitent les recalculs au périmètre utile.

**Des opérations économiques transactionnelles.** Les modèles de mutation ouvrent des contextes d'opération et prévoient une isolation sérialisable pour les écritures concurrentes. Les filtres d'instance et contrôles de lecture accompagnent les services métier.

1. Créer et configurer une instance de serveur depuis l'administration.
2. Accueillir le joueur, choisir son personnage et suivre son arrivée dans le monde.
3. Interagir avec les métiers, inventaires, banques, véhicules et logements.
4. Faire valider les actions par les services métier du serveur.
5. Suivre les états et administrer les instances depuis les interfaces connectées.

</details>

[Explorer le projet ↗](https://floriansola.fr/projects/onerp-framework)

[![StaffingOS — Relier missions, temps, frais et préparation des sorties financières.](assets/showcase/staffingos-fr.svg)](https://floriansola.fr/projects/staffingos)

StaffingOS relie les missions chez les clients, les temps, les frais et les absences aux étapes de validation et de préparation financière. Les espaces salarié et gestionnaire partagent les dossiers et leurs règles d'accès.

<details>
<summary>Architecture et parcours</summary>

**Un dossier, plusieurs responsabilités.** Le salarié, le responsable, les RH et la comptabilité interviennent sur les mêmes dossiers avec des droits et des périmètres explicites. Les règles de mission, de temps et d'absence sont partagées entre interfaces.

**Des écritures traçables.** La création d'une mission associe empreinte de commande, versions, audit et événements durables dans une transaction. Les reprises distinguent une nouvelle action du rejeu d'une action déjà enregistrée.

1. Enregistrer le client, son site, le besoin et la personne affectée.
2. Créer la mission avec ses dates et ses versions tarifaires.
3. Saisir les temps, frais et demandes d'absence depuis les espaces autorisés.
4. Examiner les demandes et exceptions dans les circuits de validation.
5. Préparer les lots de prépaie et préfacturation, puis enregistrer les preuves de règlement.

</details>

[Explorer le projet ↗](https://floriansola.fr/projects/staffingos)

[![RoadTripper — Un programme commun, une carte et un copilote pour voyager à plusieurs.](assets/showcase/roadtripper-fr.svg)](https://floriansola.fr/projects/roadtripper)

Un carnet de voyage partagé pour construire ses journées, explorer les lieux sur une carte, organiser le groupe et suivre ses dépenses. Le copilote propose des changements que les voyageurs peuvent relire avant de les adopter.

<details>
<summary>Architecture et parcours</summary>

**Le jour reste le point d'ancrage.** L'accueil, le programme et la carte partagent la journée et les identifiants d'étapes. Sur mobile, la prochaine action précède les outils secondaires ; une fiche se consulte avant d'être modifiée.

**Un calcul commun au client et au serveur.** Le domaine du carnet reste indépendant de l'interface. Hector, compilé en WebAssembly, porte les calculs déterministes de planning, budget et progression ; la passerelle valide à nouveau les données reçues.

1. Composer le voyage — Créer un carnet avec les dates et les préférences, répartir les étapes par journée, puis ajouter les lieux, pauses et nuitées.
2. Passer du programme à la carte — Choisir une journée, ouvrir une étape en lecture et la retrouver sur la carte sans perdre sa sélection. Calculer ou actualiser le trajet quand un fournisseur est configuré.
3. Préparer le départ ensemble — Inviter les membres avec un rôle, affecter les voyageurs aux voitures, vérifier la préparation et rassembler réservations, documents et budget.
4. Faire évoluer le parcours — Proposer un lieu au groupe ou demander au copilote un détour. Relire les changements sur le carnet courant avant leur adoption ; partager sa position seulement après accord.
5. Garder les comptes lisibles — Enregistrer les dépenses, leurs parts et les remboursements déclarés ; distinguer les montants engagés, estimés et réellement saisis.

</details>

[Explorer le projet ↗](https://floriansola.fr/projects/roadtripper)

[![Poisson Engine — Un écosystème vivant simulé dans le navigateur.](assets/showcase/poisson-engine-fr.svg)](https://floriansola.fr/projects/poisson-engine)

Poisson simule bancs, prédation, métabolisme et mutations dans le navigateur. Le moteur sépare le calcul WebGPU/CPU du rendu WebGL/Canvas2D et sert des modes d’observation, de sandbox et de jeu.

<details>
<summary>Architecture et parcours</summary>

**Calcul et rendu évoluent séparément.** WebGPU accélère le calcul de simulation, avec un chemin CPU quand il est indisponible. Le rendu choisit WebGL ou Canvas2D. Cette séparation permet d’adapter le travail et la présentation aux capacités du navigateur.

**Organiser les données pour le parallélisme.** Tableaux typés, structures SoA, grille spatiale, prefix-sum et réordonnancement rapprochent les agents voisins en mémoire. Le pipeline GPU traite les forces de banc et de chasse avant l’intégration physique.

1. Choisir un mode et observer les bancs, prédateurs et ressources de l’écosystème.
2. Modifier les paramètres et suivre les effets sur les déplacements, l’énergie et la reproduction.
3. Explorer génétique, mutations et rapports entre espèces.
4. Jouer avec progression, capacités, missions et économie, ou inspecter la simulation.

</details>

[Explorer le projet ↗](https://floriansola.fr/projects/poisson-engine)

## La carte de l’atelier

![Code, produits, mondes et opérations ; Hector fournit le moteur WASM de RoadTripper.](assets/showcase/ecosystem-fr.svg)

**Un lien concret entre les terrains :** RoadTripper utilise Hector en WebAssembly pour ses calculs de planning, de budget et de progression.

## Tout l’atelier

**33 projets**, organisés en quatre terrains. Produits, recherche, outils et collaborations.

<details>
<summary><strong>Moteurs, IA & agents</strong> · 9 projets</summary>

| Projet | Domaine |
| :--- | :--- |
| [AINDEX](https://floriansola.fr/projects/aindex) | Les agents opèrent. Les humains supervisent le projet. |
| [HECTOR](https://floriansola.fr/projects/hector) | Un langage pour exprimer les comportements, compiler et examiner les contrats. |
| [Continuum](https://floriansola.fr/projects/continuum) | Apprendre à naviguer, puis mesurer les décisions dans un laboratoire reproductible. |
| [PromptVault](https://floriansola.fr/projects/promptvault) | Transformer les prompts d’une équipe en outils réutilisables |
| [Matchr](https://floriansola.fr/projects/matchr) | Une offre, un CV ciblé, un dossier de candidature suivi. |
| [ModelRisk Observatory · GeopolAI](https://floriansola.fr/projects/geopolai) | Comparer les réponses de modèles IA sur des scénarios contrôlés |
| [AISelector](https://floriansola.fr/projects/ai-selector) | Un contrat commun pour appeler plusieurs fournisseurs IA |
| [Vouch](https://floriansola.fr/projects/vouch) | Préparer des réponses de sécurité à partir de sources traçables |
| [Vision Security Lab](https://floriansola.fr/projects/vision-security-lab) | Observer des comportements automatisés à partir de l’image. |

</details>

<details>
<summary><strong>Produits métier & collaboration</strong> · 6 projets</summary>

| Projet | Domaine |
| :--- | :--- |
| [OneRP](https://floriansola.fr/projects/onerp-framework) | Un socle SaaS pour exploiter des mondes roleplay FiveM. |
| [SaleCast](https://floriansola.fr/projects/salecast) | Relier les canaux de vente et préparer le prochain réapprovisionnement. |
| [StaffingOS](https://floriansola.fr/projects/staffingos) | Relier missions, temps, frais et préparation des sorties financières. |
| [RoadTripper](https://floriansola.fr/projects/roadtripper) | Un programme commun, une carte et un copilote pour voyager à plusieurs. |
| [PartyFlow](https://floriansola.fr/projects/partyflow) | Créer un salon, réunir les joueurs et enchaîner les défis |
| [Racine](https://floriansola.fr/projects/racine) | Un espace familial pour garder les liens et les souvenirs |

</details>

<details>
<summary><strong>Mondes, jeux & simulation</strong> · 13 projets</summary>

| Projet | Domaine |
| :--- | :--- |
| [FantasyOnline](https://floriansola.fr/projects/fantasy-online) | Un monde fantasy persistant, du terrain généré aux règles serveur. |
| [FantasyOnline.Shared](https://floriansola.fr/projects/fantasy-online-shared) | Partager les contrats et les règles, avec une adoption explicite par jeu. |
| [Nexus / Reclaim City](https://floriansola.fr/projects/nexus) | Récupérer des épaves et reconstruire un district à son image. |
| [SurvivalKingdom](https://floriansola.fr/projects/survival-kingdom) | Relier la survie, un monde multijoueur et les services qui le font durer. |
| [Survival Unreal](https://floriansola.fr/projects/survival-acfu) | Un monde de survie relié à ses propres services de jeu. |
| [REWORLD](https://floriansola.fr/projects/reworld) | Composer un atlas, relier ses territoires et écrire leur histoire. |
| [MANDATE EARTH](https://floriansola.fr/projects/mandate-earth) | Préparer un plan, engager des ressources et en suivre les conséquences. |
| [Symbiont](https://floriansola.fr/projects/symbiont) | Faire grandir une colonie sans épuiser le monde qui la nourrit. |
| [Poisson Engine](https://floriansola.fr/projects/poisson-engine) | Un écosystème vivant simulé dans le navigateur. |
| [Ultra RP](https://floriansola.fr/projects/ultra-rp-sbox) | Un monde roleplay s&box, du métier du joueur aux outils d’exploitation |
| [Development Tycoon](https://floriansola.fr/projects/development-tycoon) | Concevoir la croissance d’un studio logiciel comme un jeu de gestion. |
| [Red Dead Roleplay](https://floriansola.fr/projects/red-dead-roleplay) | Composer un monde roleplay autour des personnages et des interactions. |
| [V-Multi / SARP](https://floriansola.fr/projects/gaming-platform) | Un parcours fondateur dans le multijoueur et les mondes communautaires. |

</details>

<details>
<summary><strong>Infrastructure, outils & parcours</strong> · 5 projets</summary>

| Projet | Domaine |
| :--- | :--- |
| [VPS Command Center](https://floriansola.fr/projects/vps-command-center) | Relier la santé des services aux décisions d’exploitation. |
| [Infrastructure auto-hébergée](https://floriansola.fr/projects/self-hosted-infrastructure) | Organiser l’hébergement, la livraison et la reprise des produits. |
| [Portfolio Engineering](https://floriansola.fr/projects/portfolio-engineering) | Transformer les problèmes récurrents en composants réutilisables. |
| [Gecko IoT](https://floriansola.fr/projects/gecko-iot) | Une expérience professionnelle au contact du logiciel embarqué. |
| [Intégrations & archives](https://floriansola.fr/projects/integrations-archives) | Conserver les adaptateurs, les essais et les premières versions. |

</details>

---

[Site personnel](https://floriansola.fr) · [Notes et articles](https://floriansola.fr/blog) · [English](README.en.md)

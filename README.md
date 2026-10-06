![HectorLayak — Comprendre. Construire. Faire vivre.](assets/showcase/hero-fr.svg)

<p align="center"><a href="#projets-choisis">Six projets</a> · <a href="#la-carte-de-latelier">La carte</a> · <a href="#tout-latelier">33 projets</a> · <a href="https://floriansola.fr">Studio &amp; services ↗</a> · <a href="README.en.md">English</a></p>

Je construis des outils d’IA appliquée, des plateformes .NET et des systèmes temps réel. Mes projets explorent l’orchestration d’agents, les contrats exécutables, les moteurs réseau et la simulation, avec un fil rouge : maîtriser l’état, les performances et les frontières entre composants.

**C# / .NET · Rust · Python · TypeScript · C / C++**

## Projets choisis

[![AINDEX — Confier le travail aux agents. Garder la maîtrise du projet.](assets/captures/aindex-supervision.jpg)](projects/aindex.md)

**Confier le travail aux agents. Garder la maîtrise du projet.**

AINDEX organise le développement avec des agents autour d’un même projet. Un objectif devient des missions reliées à un périmètre, aux dépendances du code et aux décisions à prendre. L’équipe peut suivre le travail, examiner les changements et intervenir là où son jugement compte.

*Supervision réelle · projet fictif en mode démonstration.*

<details>
<summary>Architecture et idées</summary>

**Une mission reliée au code.** Objectif, périmètre et dépendances partagent le même contexte. L’index relie symboles, appels et références utiles au travail demandé.

**Le bon contexte au bon moment.** Une capsule rassemble les obligations et les sources pertinentes. Sa provenance et sa fraîcheur restent consultables pendant la mission.

**La supervision au service de la décision.** Le Studio montre ce qui avance, ce qui change et ce qui mérite attention. L’équipe retrouve questions, résultats et éléments de revue dans le même parcours.

</details>

[Explorer le projet ↗](projects/aindex.md)

[![HECTOR — Décrire le besoin. Construire la mécanique.](assets/showcase/hector-fr.svg)](projects/hector.md)

**Décrire le besoin. Construire la mécanique.**

HECTOR part d’une idée : l’auteur doit pouvoir exprimer le comportement attendu, ses contraintes et les transformations autorisées. Types, unités, effets et contrats donnent une forme explicite à cette intention. Le langage vise aussi les agents : leurs propositions deviennent examinables par le compilateur.

<details>
<summary>Architecture et idées</summary>

**Le comportement avant la mécanique.** Déclarer les valeurs, les résultats et les obligations. L’auteur précise aussi les libertés : représentation, fusion ou ordre indépendant.

**Un langage pour humains et agents.** Les types, effets et contrats rendent les propositions analysables. L’agent propose un changement ; le compilateur expose les contradictions qu’il sait détecter.

**Un noyau réutilisable.** Les mêmes sources produisent des bibliothèques natives et WebAssembly. Les interfaces et les identités de compilation accompagnent leur intégration dans les applications.

</details>

[Explorer le projet ↗](projects/hector.md)

[![OneRP — Un socle SaaS pour exploiter des mondes roleplay FiveM.](assets/showcase/onerp-framework-fr.svg)](projects/onerp-framework.md)

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

[Explorer le projet ↗](projects/onerp-framework.md)

[![StaffingOS — Relier missions, temps, frais et préparation des sorties financières.](assets/showcase/staffingos-fr.svg)](projects/staffingos.md)

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

[Explorer le projet ↗](projects/staffingos.md)

[![RoadTripper — Un programme commun, une carte et un copilote pour voyager à plusieurs.](assets/showcase/roadtripper-fr.svg)](projects/roadtripper.md)

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

[Explorer le projet ↗](projects/roadtripper.md)

[![Poisson Engine — Un écosystème vivant simulé dans le navigateur.](assets/showcase/poisson-engine-fr.svg)](projects/poisson-engine.md)

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

[Explorer le projet ↗](projects/poisson-engine.md)

## La carte de l’atelier

![Code, produits, mondes et opérations ; Hector fournit le moteur WASM de RoadTripper.](assets/showcase/ecosystem-fr.svg)

**Un lien concret entre les terrains :** RoadTripper utilise Hector en WebAssembly pour ses calculs de planning, de budget et de progression.

## Tout l’atelier

**33 projets**, organisés en quatre terrains. Produits, recherche, outils et collaborations.

<details>
<summary><strong>Moteurs, IA & agents</strong> · 9 projets</summary>

| Projet | Domaine |
| :--- | :--- |
| [AINDEX](projects/aindex.md) | Les agents opèrent. Les humains supervisent le projet. |
| [HECTOR](projects/hector.md) | Un langage pour exprimer les comportements, compiler et examiner les contrats. |
| [Continuum](projects/continuum.md) | Apprendre à naviguer, puis mesurer les décisions dans un laboratoire reproductible. |
| [PromptVault](projects/promptvault.md) | Transformer les prompts d’une équipe en outils réutilisables |
| [Matchr](projects/matchr.md) | Une offre, un CV ciblé, un dossier de candidature suivi. |
| [ModelRisk Observatory · GeopolAI](projects/geopolai.md) | Comparer les réponses de modèles IA sur des scénarios contrôlés |
| [AISelector](projects/ai-selector.md) | Un contrat commun pour appeler plusieurs fournisseurs IA |
| [Vouch](projects/vouch.md) | Préparer des réponses de sécurité à partir de sources traçables |
| [Vision Security Lab](projects/vision-security-lab.md) | Observer des comportements automatisés à partir de l’image. |

</details>

<details>
<summary><strong>Produits métier & collaboration</strong> · 6 projets</summary>

| Projet | Domaine |
| :--- | :--- |
| [OneRP](projects/onerp-framework.md) | Un socle SaaS pour exploiter des mondes roleplay FiveM. |
| [SaleCast](projects/salecast.md) | Relier les canaux de vente et préparer le prochain réapprovisionnement. |
| [StaffingOS](projects/staffingos.md) | Relier missions, temps, frais et préparation des sorties financières. |
| [RoadTripper](projects/roadtripper.md) | Un programme commun, une carte et un copilote pour voyager à plusieurs. |
| [PartyFlow](projects/partyflow.md) | Créer un salon, réunir les joueurs et enchaîner les défis |
| [Racine](projects/racine.md) | Un espace familial pour garder les liens et les souvenirs |

</details>

<details>
<summary><strong>Mondes, jeux & simulation</strong> · 13 projets</summary>

| Projet | Domaine |
| :--- | :--- |
| [FantasyOnline](projects/fantasy-online.md) | Un monde fantasy persistant, du terrain généré aux règles serveur. |
| [FantasyOnline.Shared](projects/fantasy-online-shared.md) | Partager les contrats et les règles, avec une adoption explicite par jeu. |
| [Nexus / Reclaim City](projects/nexus.md) | Récupérer des épaves et reconstruire un district à son image. |
| [SurvivalKingdom](projects/survival-kingdom.md) | Relier la survie, un monde multijoueur et les services qui le font durer. |
| [SurvivalUnreal](projects/survival-unreal.md) | Un monde de survie relié à ses propres services de jeu. |
| [REWORLD](projects/reworld.md) | Composer un atlas, relier ses territoires et écrire leur histoire. |
| [MANDATE EARTH](projects/mandate-earth.md) | Préparer un plan, engager des ressources et en suivre les conséquences. |
| [Symbiont](projects/symbiont.md) | Faire grandir une colonie sans épuiser le monde qui la nourrit. |
| [Poisson Engine](projects/poisson-engine.md) | Un écosystème vivant simulé dans le navigateur. |
| [Ultra RP](projects/ultra-rp-sbox.md) | Un monde roleplay s&box, du métier du joueur aux outils d’exploitation |
| [Development Tycoon](projects/development-tycoon.md) | Concevoir la croissance d’un studio logiciel comme un jeu de gestion. |
| [Red Dead Roleplay](projects/red-dead-roleplay.md) | Composer un monde roleplay autour des personnages et des interactions. |
| [V-Multi / SARP](projects/gaming-platform.md) | Un parcours fondateur dans le multijoueur et les mondes communautaires. |

</details>

<details>
<summary><strong>Infrastructure, outils & parcours</strong> · 5 projets</summary>

| Projet | Domaine |
| :--- | :--- |
| [VPS Command Center](projects/vps-command-center.md) | Relier la santé des services aux décisions d’exploitation. |
| [Infrastructure auto-hébergée](projects/self-hosted-infrastructure.md) | Organiser l’hébergement, la livraison et la reprise des produits. |
| [Portfolio Engineering](projects/portfolio-engineering.md) | Transformer les problèmes récurrents en composants réutilisables. |
| [Gecko IoT](projects/gecko-iot.md) | Une expérience professionnelle au contact du logiciel embarqué. |
| [Intégrations & archives](projects/integrations-archives.md) | Conserver les adaptateurs, les essais et les premières versions. |

</details>

---

[Studio & services](https://floriansola.fr) · [Notes et articles](https://floriansola.fr/blog) · [English](README.en.md)

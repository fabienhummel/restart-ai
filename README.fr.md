# ReStart AI

**Un coach IA local pour la recherche d'emploi, la reconversion professionnelle et les personnes touchées par les suppressions de postes liées à l'intelligence artificielle.**

[Français](README.fr.md) · [English](README.md)

> **Statut : concept / AI Entry.** ReStart AI est une application envisagée, pas encore un logiciel opérationnel. Les fonctionnalités et intégrations décrites ici ne sont pas implémentées.


## Documentation détaillée

| Sujet | Français | English |
| --- | --- | --- |
| Architecture | [Architecture](docs/architecture.fr.md) | [Architecture](docs/architecture.md) |
| Fonctionnalités | [Fonctionnalités](docs/features.fr.md) | [Features](docs/features.md) |
| Scénarios | [Cas d'usage](docs/use-cases.fr.md) | [Use cases](docs/use-cases.md) |
| Confidentialité et sécurité | [Confidentialité et sécurité](docs/privacy-security.fr.md) | [Privacy & safety](docs/privacy-security.md) |
| Développement | [Feuille de route](docs/roadmap.fr.md) | [Roadmap](docs/roadmap.md) |

## Le problème

Une perte d'emploi ou une reconversion entraîne de nombreuses démarches : faire le bilan de ses compétences, explorer de nouveaux métiers, rechercher des offres, adapter son CV, rédiger des lettres de motivation, suivre les candidatures, préparer les entretiens et identifier les formations utiles.

Les personnes concernées par l'automatisation et l'IA doivent parfois réévaluer leur parcours et leurs compétences transférables. Les outils existants traitent souvent des étapes isolées, tandis que le recours à des services en ligne peut soulever des questions de confidentialité.

## Le concept

**ReStart AI** est un projet d'agent IA personnel visant à accompagner l'ensemble d'un parcours de recherche d'emploi ou de transition professionnelle. Il s'adresse en particulier aux personnes dont l'emploi a été supprimé ou transformé par l'IA et l'automatisation, sans se limiter à ce public.

Au lieu de simplement générer du texte, l'agent pourrait planifier des démarches, utiliser des outils autorisés, examiner leurs résultats et proposer l'étape suivante. Les décisions importantes resteraient entre les mains de l'utilisateur.

### Fonctionnalités envisagées

| Module | Fonction prévue |
| --- | --- |
| Profil professionnel | Constituer un inventaire vérifié des expériences et compétences, identifier les acquis transférables et explorer des métiers. |
| Recherche d'emploi | Rechercher sur des sources autorisées, filtrer les offres, supprimer les doublons et expliquer les correspondances. |
| Atelier de candidature | Adapter des CV et lettres sans inventer de faits ; exporter en DOCX, ODT et PDF modifiables lorsque le format le permet. |
| Suivi des candidatures | Suivre les étapes, relances, entretiens, échéances et versions des documents envoyés. |
| Préparation aux entretiens | Simuler des entretiens adaptés aux postes et fournir des retours constructifs. |
| Reconversion | Identifier les écarts de compétences et proposer des pistes de formation. |
| Organisation | Préparer tâches et rappels ; proposer des connexions facultatives à Notion, à un agenda ou à une messagerie. |
| Évolution des métiers | Examiner l'impact possible de l'automatisation sur des tâches, sans prétendre prédire les suppressions d'emplois. |

### Exemple de fonctionnement agentique

1. L'utilisateur indique sa région, les métiers souhaités, sa disponibilité et ses critères.
2. L'agent recherche des offres sur des sources autorisées et élimine les doublons.
3. Il compare les annonces au parcours professionnel vérifié et justifie sa sélection.
4. Pour les offres validées, il prépare des brouillons de CV et de lettres de motivation.
5. Il propose des relances et une mise à jour du tableau de suivi.
6. **Aucune candidature, aucun courriel ni document personnel ne serait envoyé sans accord explicite.**

## Architecture locale envisagée

```text
Utilisateur / interface web
          |
Agent coordinateur (Python)
          |
          +-- Bilan de compétences et carrières
          +-- Recherche d'offres (sources autorisées)
          +-- Génération documentaire (DOCX / ODT / PDF)
          +-- Suivi des candidatures et rappels
          +-- Connecteurs facultatifs (Notion / agenda / e-mail)
          |
LLM local via Ollama + recherche documentaire privée
          |
Stockage local de l'application
```

Technologies candidates : Python, FastAPI, Ollama, modèle de langage open weight quantifié adapté aux ressources disponibles, SQLite dans un premier temps, bibliothèques de génération documentaire, RAG facultatif et déploiement Docker éventuel. **Les choix définitifs restent à étudier.**

Plusieurs fonctions spécialisées pourraient partager un même modèle local plutôt que nécessiter plusieurs LLM simultanément.

## Configuration ASUS de référence

La **ASUS GeForce RTX 5060 Ti 16 Go** et la **ASUS PRIME B860-PLUS WIFI** constituent une **configuration matérielle cible envisagée**, et non du matériel sur lequel le projet aurait déjà été testé. Un PC complet nécessite également un processeur compatible, de la mémoire, du stockage et d'autres composants.

L'objectif est de privilégier l'inférence GPU locale sur un PC grand public, avec des modèles plus légers sur les machines modestes. Aucune mesure de performances ni validation matérielle n'a encore été effectuée pour ReStart AI.

## Confidentialité, sécurité et confiance

- Traitement et stockage locaux par défaut ; connexions cloud facultatives avec consentement.
- Validation explicite avant l'envoi d'une candidature, d'un e-mail ou d'informations personnelles.
- Aucune invention de diplômes, d'expériences ou de compétences.
- Explication des rapprochements entre profils et offres et signalement des incertitudes.
- Permissions limitées des outils, journal des actions et maîtrise des données par l'utilisateur.
- Respect des conditions d'utilisation des plateformes et des règles de protection des données.

## Feuille de route

- **Phase 0 — Concept (actuelle) :** vision, cas d'usage, architecture, confidentialité et étude de faisabilité.
- **Phase 1 — Prototype :** LLM local, profil professionnel simple et premier scénario agentique encadré.
- **Phase 2 — MVP :** import d'offres, documents éditables et suivi des candidatures.
- **Phase 3 — Intégrations :** Notion, e-mail, calendrier et accompagnement enrichi, facultatifs.
- **Phase 4 — Consolidation :** accessibilité, sécurité, tests, évaluation des modèles et retours utilisateurs.

## ASUS Agent Computer Challenge

Ce dépôt présente un **concept destiné à la catégorie AI Entry** du concours ASUS Agent Computer Challenge. Il ne prétend pas disposer d'un agent finalisé, d'intégrations fonctionnelles ni de résultats de tests.

## Principes du projet

ReStart AI a vocation à être accessible, transparent et, à terme, open source. **La licence logicielle reste à choisir** : rendre ce dépôt public ne signifie pas que sa réutilisation soit déjà autorisée.

---

**English:** [Read the full English presentation](README.md).

# Feuille de route

[Français](roadmap.fr.md) · [English](roadmap.md)

Cette feuille de route est **indicative** et ne constitue pas une promesse de livraison.

| Étape | Résultat envisagé | Preuve attendue |
| --- | --- | --- |
| 0 — Concept (actuel) | Problème, périmètre, architecture, scénarios et garanties | Documentation relue |
| 1 — Faisabilité | Fichiers Markdown depuis le navigateur, OAuth de stockage, tests Ollama et IA cloud, accès aux offres et exports | Notes techniques et audit des flux |
| 2 — Prototype | Profil professionnel, offre sourcée, sélection d'outils par l'agent | Démonstration locale reproductible |
| 3 — MVP | Brouillons personnalisés, tableau de suivi et validations | Test complet sur données fictives |
| 4 — Intégrations | Notion, agenda, messagerie et autres sources autorisées, en option | Tests de permissions et d'erreurs |
| 5 — Consolidation | Sécurité, accessibilité, portabilité, évaluations et documentation | Résultats de tests et liste de vérification |

## Pistes d'évaluation
- Fidélité des CV au parcours réellement fourni.
- Exactitude des références aux annonces.
- Nombre d'actions non autorisées (**objectif : zéro**).
- Qualité des exports DOCX/ODT.
- Consommation de ressources, temps de réponse et stabilité des modèles locaux.
- Facilité à consulter, corriger et supprimer les données professionnelles.

## Décisions ouvertes
Adaptateurs de stockage, compatibilité des navigateurs, gestion OAuth et clés API, compagnon local éventuel ; choix des modèles ; framework ou orchestrateur Python léger ; systèmes d'exploitation compatibles ; accès aux sources d'offres et conditions d'utilisation ; licence logicielle ; accessibilité ; modèles de documents.

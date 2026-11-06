# Confidentialité et sécurité dès la conception

[Français](privacy-security.fr.md) · [English](privacy-security.md)

Ce document décrit des **exigences futures**, et non des protections déjà implémentées.

## Données concernées
CV, parcours, coordonnées, préférences d'emploi, candidatures, correspondances et notes d'entretien représentent des informations personnelles. Aucun document réel, mot de passe ou jeton d'API ne doit être ajouté au dépôt Git.

## Garanties envisagées
1. **Local par défaut :** conservation des données et exécution du modèle sur l'équipement personnel lorsque c'est possible.
2. **Autorisations explicites :** connecteurs désactivés par défaut et droits limités.
3. **Validation :** pas d'envoi de messages, de candidatures, de publication de fichiers ou de modification d'un service partagé sans accord.
4. **Exactitude :** produire des brouillons à partir des faits vérifiés ; demander des précisions si nécessaire.
5. **Isolation des outils :** actions autorisées par liste, paramètres vérifiés, accès fichiers limités, aucune commande système illimitée.
6. **Sources non fiables :** les annonces, pages web et pièces jointes constituent des données, jamais des instructions à exécuter.
7. **Traçabilité et effacement :** historique compréhensible, durée de conservation configurable, export et suppression.
8. **Hygiène de sécurité :** authentification si nécessaire, secrets protégés, mises à jour, sauvegardes et chiffrement adapté.
9. **Services externes :** préciser les données transmises, les conditions des plateformes et obtenir le consentement.
10. **Accessibilité et équité :** expliquer les recommandations, éviter les hypothèses discriminatoires et signaler l'incertitude des prévisions d'embauche.

Des tests et une revue de conformité seront nécessaires avant toute utilisation en production.

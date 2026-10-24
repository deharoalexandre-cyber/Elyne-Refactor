# Architecture — Elyne Refactor

[English](architecture.en.md) · [Présentation](../README.md)

## Flux simplifié

Dépôt autorisé → analyse statique et contexte → propositions de modèles → comparaison et contrôles → rapport pour revue humaine.

## Composants et frontières

- Le pipeline annoncé combine sandbox de travail, analyse déterministe, recherche documentaire et comparaison de propositions issues de plusieurs modèles locaux.
- Les sorties peuvent prendre la forme de correctifs et de rapports structurés. La signature éventuelle atteste un artefact produit ; elle ne prouve pas à elle seule la justesse d'un correctif.
- Le déploiement local et la possibilité d'isolement réseau sont des objectifs d'architecture. Les intégrations CLI, API, IDE et CI dépendent de la version et du profil installés.

Ce schéma textuel décrit l'architecture du produit. Il ne remplace pas une vérification sur un build, un matériel et une configuration précis. Les [éléments de preuve](evidence.md) indiquent ce qui a été effectivement documenté.

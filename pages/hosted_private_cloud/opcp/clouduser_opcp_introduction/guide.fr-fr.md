---
title: "Présentation du produit OPCP"
excerpt: "Ce guide a pour but de vous présenter le produit OPCP"
updated: 2025-02-12
---

## Objectif

Ce document vise à fournir aux **Cloud users** des instructions claires pour utiliser les fonctionnalités de la solution **OPCP**, via le composant Openstack Horizon de manière efficace, telles que la gestion des ressources, la gestion des instances, la configuration des réseaux ainsi que la gestion des incidents.

## Présentation du produit OPCP


La solution OPCP (On Prem Cloud Platform) est une solution clé en main mise en place par OVHcloud afin de déployer une infrastructure Cloud en datacenter des clients qui sont soumis à des fortes contraintes règlementaires ou qui souhaitent conserver le contrôle total de leur données et opérations.

Il  s’agit  d’une  solution  clé  en  main  basée  sur  des  serveurs  physiques,  et  livrée précablée depuis l’usine OVHcloud. Trois rôles interviennent sur l’écosystème OPCP : 

| Rôle | Description |
|------|-------------|
| DC Operator | L'opérateur en datacentre, en charge de la maintenance du hardware. Il peut gérer l'inventaire, enregistrer les changements apportés à l'infrastructure, et identifier qui est l'utilisateur actuel du serveur |
| IT Administrator | Personne en charge de l'attributions et la maintenance des ressources livrées avec la baie OPCP. |
| Cloud user | Utilisateur en self-service de la solution OPCP. Il peut consommer des ressources dans les limites des droits et quotas fournis par l'IT administrator |


Ce guide s'adresse  aux  **Cloud user**  de  l’offre  OPCP.  Cela  englobe  la création   et  la  gestion  d'instances,  la  configuration   des  réseaux  privés  et  la 
surveillance de l'utilisation des ressources (telles que le processeur et la mémoire). Ces actions sont soumises à des autorisations établies par l'**IT Administrator**.

## Glossaire

| Terme      | Signification      |
| ------------- | ------------- |
| Openstack Horizon | Interface web graphique d'Openstack. | 
| Netbox | Un outil utilisé pour la gestion de l'infrastructure réseau. | 
| Grafana | Un outil utilisé pour visualiser et surveiller les données en temps réel. | 
| Instance | Un serveur dédié  | 
| Projet  | Un environnement isolé dans lequel un groupe d'utilisateurs peut gérer des ressources  | 
| IP flottante | Une  adresse  IP  publique  qui  peut  être  attribuée  dynamiquement  à  une instance pour la rendre accessible depuis l'extérieur du réseau privé.  | 
| Keycloak | Une solution de gestion des identités et des accès. | 
| IAM | Gestion des identités et des accès | 
| API  | Interface programmable via REST |
|   Compute | Ressources de calcul | 
| Pare-feu  | Un dispositif de sécurité qui contrôle le trafic réseau entrant et sortant | 
| Gabarit (Flavor) | La configuration matérielle. | 
| Subnet | Sous-réseau | 
| Gateway(passerelle) | Un dispositif de connexion qui permet de faire le lien entre deux réseaux différents.  | 
| CIDR( Classless Inter-Domain Routing)  | un   format   d'adressage   réseau   utilisé   pour   représenter   des   plages d'adresses IP | 

## Rôles et responsabilités des Cloud users

Le rôle d'un utilisateur final dans la solution OPCP consiste à gérer et exploiter les ressources machine qui lui sont attribuées. Cela comprend la création et la gestion des instances, la mise en place de réseaux privés, la surveillance de l'utilisation des ressources (CPU et RAM) dans les limites de ses quotas. Ceci englobe également les actions suivantes :
* Lancer des instances 
* Arrêter, suspendre, ou redémarrer des instances 
* Associer des adresses IP flottantes 
* Gérer les réseaux 
* Prendre des instantanés snapshots
* Gérer les clés SSH 
* Redimensionner des instances 
* Consulter les quotas et l'utilisation des ressources

## Aller plus loin

Si vous avez besoin d'une formation ou d'une assistance technique pour la mise en oeuvre de nos solutions, contactez votre commercial ou cliquez sur [ce lien](/links/professional-services) pour obtenir un devis et demander une analyse personnalisée de votre projet à nos experts de l’équipe Professional Services.

Échangez avec notre [communauté d'utilisateurs](/links/community).

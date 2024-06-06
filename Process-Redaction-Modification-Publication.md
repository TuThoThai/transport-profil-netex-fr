---
title: "Les profils français des normes européennes : processus technique de rédaction, modification et publication"
date: 2024-06-06T10:00:00+02:00
draft: true
autonumbering: true
---

# Introduction
Ce document a été rédigé dans le cadre des travaux de normalisation menés par le Bureau de normalisation pour les transports, les routes et leurs aménagements (BNTRA), au sein de la Commission de Normalisation Transport Public (CN03) et, plus particulièrement, de son Groupe de Travail sur l’information voyageur et l’exploitation des services de mobilités (GT7).

Le groupe de travail a été mandaté pour piloter l’usage de l’outil [GitHub](https://github.com/) pour la rédaction, la modification et la publication des profils français (aussi appelés profils France) des normes européennes ayant trait au Transport Public. La publication de ces profils se faisant sur le site [normes.transport.data.gouv.fr](https://normes.transport.data.gouv.fr/) (ci-après nommé "site"), ce document a été rédigé avec l'appui des équipes du [Point d'Accès National aux données de transport](https://transport.data.gouv.fr/) (ci-après nommé "PAN") qui ont la gestion du site de publication à ce jour.

Ce document a un double objectif :
- Accompagner et documenter les travaux du GT7,
- Proposer un processus technique de travail avec l'outil GitHub aux autres GTs de la CN03 et autres groupes concernés pour leurs travaux.


# Périmètre de publication du site
À ce jour, il a été décidé que feront l’objet de publication sur le site l’ensemble des profils France des normes européennes produits par le GT7 et GT9, à savoir :
- Le profil français  de la norme européenne NeTEx et ses différents composants (appelés “sous-profils”)
  - Profil France - Éléments communs
  - Profil France - Description des arrêts
  - Profil France - Horaires
  - Profil France - Description des réseaux
  - Profil France - Accessibilité
  - Profil France - Tarifs
  - Profil France - Parkings (porté par le GT9)
- le profil français de la norme européenne SIRI.

À terme, les schémas nationaux issus des travaux de la Fabrique des Mobilités seront également publiés et référencés sur le PAN. Cependant, le site exact de publication n’a pas encore été défini. Pour rappel, ces schémas nationaux sont :
- Chapeau standard MAS
- Standard Covoiturage - Open Carpooling Service Standard (OCSS)
- Standard Compte Mobilité Standardisé

Cependant, le processus détaillé ci-après a pour vocation d’être élargi à l’ensemble des travaux des GTs de la CN03. Les listes ci-dessus seront donc amenées à évoluer.


# Les profils de normes, standards, spécifications techniques et schémas nationaux
## Définitions
**Norme** : document établi par un consensus et approuvé par un organisme reconnu (ex. AFNOR, CEN), qui fournit, pour des usages communs et répétés, des règles, des lignes directrices ou des caractéristiques, pour des activités ou leurs résultats, garantissant un niveau d'ordre optimal dans un contexte donné. Ces normes sont établies au sein de groupes de travail ou comités techniques d’instances de normalisation. Tout changement apporté à une norme doit faire l’objet d’un vote formel au sein de ces instances de normalisation organisé auprès de leurs membres. Les normes européennes sont produites par le CEN, CENELEC ou ETSI.

> Exemple : Transmodel

**Profil de norme** : sous-ensemble défini à partir d’une norme ou d’un standard européen (CEN) qui peut comporter des règles spécifiques. Dans le cadre des travaux de la CN03, ces profils sont produits en français par ses groupes de travail. 

Dans le cas de la norme NeTEx, il existe également des sous-profils pour définir plus finement certains aspects des transports publics (ex. Accessibilité) ; leur ensemble forme le profil France de la norme NeTEx.

> Exemple : NeTEx – Profil France   et son sous profil NeTEx – Profil France - Accessibilité

**Standard** : référentiel ou ensemble de recommandations développées et préconisées par un groupe autre qu’une instance de normalisation nationale ou internationale ou non approuvé par ces dernières pour un usage national ou international. On ne parle de standard qu'à partir du moment où le référentiel a une diffusion large, on parle alors de standard de facto (standard de fait). Un standard est ouvert quand le référentiel est diffusé librement.

> Exemple : GTFS

**Spécification technique** : tout document normatif établi par une instance de normalisation (ex. CEN) qui peut co-exister avec un standard national mais ne peut entrer en conflit avec une norme existante. Ces documents sont généralement issus d’un besoin spécifique ne pouvant pas encore aboutir à une norme par manque de consensus au sein de l’ensemble des membres ou sur demande expresse des parties prenantes (ex. DG MOVE) dans le but de conserver un cycle de vie plus court d’élaboration de documents normatifs. Le plus souvent, elles sont rédigées en vue d’une future harmonisation ou pour permettre des expérimentations ou pour s’adapter à des technologies évolutives.

> Exemple : SIRI sur certaines parties

**Schéma national** : 
tout autre document issu d’un groupe de travail du BNTRA ou du PAN dont la gouvernance ne dépend pas directement d’instances de normalisation européennes ou internationales. Ces documents sont généralement issus d’un besoin spécifique de standardisation des échanges de données requises à un niveau national sans qu’il existe une norme ou standard adéquat. Ces schémas ont, le plus souvent, vocation à devenir des standards nationaux, voire des normes européennes.

> Exemple : Aménagements cyclables

Dans le reste du document, "documents techniques" fera référence aux profils de normes, standards et spécifications techniques sans distinction.

## De l'usage des profils dédiés
Si un organisme souhaite avoir un profil dédié à ses usages, il est très fortement recommandé que ce profil soit basé sur les profils nationaux publiés sur le site. Cela a pour but principal de maintenir l’interopérabilité des données échangées au niveau national. En conséquence, le profil dédié contiendra :
- Une référence explicite au profil national ayant servi de base au profil dédié,
- Les explications liées à la création de sous-ensemble de champs ou d’attributs du profil national,
- Les règles explicites du profil dédié,
- Des exemples propres au profil dédié et à sa constellation d’acteurs pour faciliter leurs échanges de données.

Il est également recommandé de ne pas republier l’intégralité du profil ayant servi de base de travail. Cela permettra :
- D'en faciliter la lecture, réduite aux seuls éléments distinctifs des parties spécifiques au profil dédié,
- De s’assurer qu’il n’existe pas de contradictions entre le profil France et le profil dédié, le premier servant de référence.

Enfin, avant d’entamer la rédaction d’un profil dédié, il est préférable de se rapprocher du groupe de travail ayant eu la charge du profil national. Un premier échange pourrait :
- Définir si un profil dédié est nécessaire,
- Aider à la prise en main du profil France,
- Soutenir le cadrage du profil dédié et sa mise en cohérence avec le profil national.


# Processus technique de rédactiion, modification et publication
Ce processus technique comprend trois phases principales pouvant être réalisées en parallèle :
- La rédaction, puis modification ou révision continue de la version de travail avec des propositions de modification libres validées par des personnes identifiées au sein des groupes de travail concernés,
- La définition d’une version « officielle » validée par l’ensemble des membres du groupe de travail concerné, avalisé par la CN03, et qui est dotée d’un numéro de version,
- La publication de la version validée sur le site.

Le schéma ci-après illustre les trois phrases :



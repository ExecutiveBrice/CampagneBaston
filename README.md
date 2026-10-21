# CampagneBaston — La Compagnie des Huit Catastrophes

**Le Médaillon de l’Omnipotence Approximative** : une campagne originale de fantasy comique pour **4 à 8 adolescents**, avec des profils maison pour **Chroniques Oubliées Fantasy 2**.

## Jouer et préparer

1. Lire la [présentation](campagne/Presentation.md), la [mission principale](campagne/Mission.md) et les [règles communes](campagne/Regles.md).
2. Laisser les joueurs choisir parmi les [huit zones](zones/README.md).
3. Préparer les [trois indices communs](indices/Indices.md) et le [final](campagne/Final.md).
4. Configurer les dialogues avec les [consignes des PNJ IA](commun/PNJ-IA.md).

Les zones restent libres. Trois scénarios permettent d’identifier le laboratoire et de terminer la mission. Chaque zone tient en moins d’une heure. Les indices sont remis dans l’ordre, indépendamment des zones : **8 positions, puis 4, puis 1**.

## Une arborescence par zone

Chaque zone possède son dossier sous `zones/` et contient **quatre fichiers complets et éditables** :

| Fichier | Contenu |
| --- | --- |
| `Scenario.md` | Accroche, lieux, déroulement, approches, résolution et remise de l’indice |
| `PNJ.md` | Quatre personnages avec objectifs, connaissances, secrets, réactions et voix |
| `Monstres.md` | Bestiaire local chiffré : DEF, PV, initiative, attaques, armes, armure, capacités et moral |
| `Objets.md` | Cinq objets à trouver, gagner ou acheter, avec prix, bonus et pouvoirs éventuels |

Exemple : [village/Scenario.md](zones/village/Scenario.md), [village/PNJ.md](zones/village/PNJ.md), [village/Monstres.md](zones/village/Monstres.md) et [village/Objets.md](zones/village/Objets.md).

## Accès aux huit zones

| Zone | Dossier |
| --- | --- |
| Grande ville | [zones/grande-ville](zones/grande-ville/Scenario.md) |
| Village | [zones/village](zones/village/Scenario.md) |
| Forêt | [zones/foret](zones/foret/Scenario.md) |
| Marécage | [zones/marecage](zones/marecage/Scenario.md) |
| Montagne | [zones/montagne](zones/montagne/Scenario.md) |
| Plaine | [zones/plaine](zones/plaine/Scenario.md) |
| Désert | [zones/desert](zones/desert/Scenario.md) |
| Plage | [zones/plage](zones/plage/Scenario.md) |

## Autres ressources

| Dossier | Contenu |
| --- | --- |
| [campagne/](campagne/README.md) | Mission, règles, final, aide MJ et correspondance des anciens chapitres |
| [commun/](commun/README.md) | Archibald, consignes IA, 18 monstres généralistes et 32 objets généralistes |
| [indices/](indices/README.md) | Textes et méthode des trois indices, préparation des supports |
| [plans/](plans/README.md) | Cartes et plans à ajouter, suivi des sources |
| [sessions/](sessions/README.md) | Modèle de journal des parties, décisions et inventaires |
| [exports/](exports/README.md) | Futurs PDF et aides de jeu imprimables |
| [archives/](archives/README.md) | Livret d’origine conservé intégralement comme archive figée |

## Faire évoluer la campagne

Modifier les fichiers de la zone concernée et les fichiers communs : ce sont les sources éditoriales de référence. L’archive d’origine ne reçoit pas ces modifications. Les références conservées aux chapitres du livret sont expliquées dans le [sommaire](campagne/README.md).

Lire [AGENTS.md](AGENTS.md) pour les contraintes et conventions. Décrire chaque évolution dans un commit et consigner les changements importants dans [CHANGELOG.md](CHANGELOG.md). Une branche et une pull request peuvent servir pour une révision à relire.

Les conversations ne sont pas synchronisées automatiquement avec GitHub. Reporter les décisions utiles dans les fichiers. Aucun plan graphique, calque ajusté ou export PDF n’est inclus dans cet import initial.

Ce dépôt contient les solutions et secrets du MJ. Préparer des documents distincts pour les joueurs ; les dossiers ne constituent pas des droits d’accès séparés.

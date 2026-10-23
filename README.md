# CampagneBaston — La Compagnie des Huit Catastrophes

**À la recherche du laboratoire introuvable** : une campagne originale de fantasy comique pour **4 à 8 adolescents**, avec des profils maison pour **Chroniques Oubliées Fantasy 2**.

## Jouer et préparer

1. Lire la [présentation](campagne/Presentation.md), la [mission principale](campagne/Mission.md) et les [règles communes](campagne/Regles.md).
2. Laisser les joueurs choisir parmi les [huit zones](zones/README.md).
3. Préparer les [trois indices communs](indices/Indices.md) et le [final](campagne/Final.md).
4. Ouvrir directement ce dossier dans NPC : [guide de lancement et format natif](campagne/NPC.md). Les [consignes des PNJ IA](zones/commun/PNJ-IA.md) restent disponibles pour les autres outils.

Les zones restent libres. Retrouver le laboratoire d’Archibald Malépine constitue la quête principale : trois scénarios permettent de réunir les trois indices et de terminer la mission. Le mage aide les joueurs à choisir leurs destinations et à lire les supports. Chaque zone tient en moins d’une heure. Les indices sont remis dans l’ordre, indépendamment des zones : **8 positions, puis 4, puis 1**.

## Ouvrir cette campagne dans NPC

La racine de ce dépôt est directement utilisable par le projet `pnj`, sans import.
Avec l'installation locale actuelle :

```sh
/Users/brice/PycharmProjects/pnj/.venv/bin/npc gui /Users/brice/WebstormProjects/CampagneBaston
```

Les 33 fiches individuelles sont dans `zones/<zone>/characters/`, avec un
`lore.md` par zone. [Le guide NPC](campagne/NPC.md) décrit les voix, les mémoires,
les secrets, les commandes et les fichiers à modifier pour faire évoluer la partie.

## Une arborescence par zone

Chaque zone possède son dossier sous `zones/` et contient **quatre fichiers complets et éditables** :

| Fichier | Contenu |
| --- | --- |
| `Scenario.md` | Accroche, lieux, déroulement, approches, résolution et remise de l’indice |
| `PNJ.md` | Quatre personnages avec objectifs, connaissances, secrets, réactions et voix |
| `Monstres.md` | Bestiaire local chiffré : DEF, PV, initiative, attaques, armes, armure, capacités et moral |
| `Objets.md` | Cinq objets à trouver, gagner ou acheter, avec prix, bonus et pouvoirs éventuels |

En complément, `characters/` contient les fiches individuelles lues directement
par NPC et `lore.md` décrit uniquement le décor observable partagé. Ces fichiers
sont édités sur place ; il n'y a aucune étape de génération ou d'import.

Exemple : [village/Scenario.md](zones/village/Scenario.md), [village/PNJ.md](zones/village/PNJ.md), [village/Monstres.md](zones/village/Monstres.md) et [village/Objets.md](zones/village/Objets.md).

## Accès aux huit zones

| Zone | Dossier |
| --- | --- |
| Grande ville — Valombre | [zones/grande-ville](zones/grande-ville/Scenario.md) |
| Village — Tilverton | [zones/village](zones/village/Scenario.md) |
| Forêt — Cormanthor | [zones/foret](zones/foret/Scenario.md) |
| Marécage — le Grand Marais | [zones/marecage](zones/marecage/Scenario.md) |
| Montagne — l’Échine du Dragon | [zones/montagne](zones/montagne/Scenario.md) |
| Plaine — la Sembie | [zones/plaine](zones/plaine/Scenario.md) |
| Désert — l’Anauroch | [zones/desert](zones/desert/Scenario.md) |
| Plage — la côte de la Mer de Lune | [zones/plage](zones/plage/Scenario.md) |

## Autres ressources

| Dossier | Contenu |
| --- | --- |
| [campagne/](campagne/README.md) | Mission, règles, final, aide MJ et correspondance des anciens chapitres |
| [commun/](zones/commun/README.md) | Archibald, consignes IA, 18 monstres généralistes et 32 objets généralistes |
| [indices/](indices/README.md) | Textes et méthode des trois indices, préparation des supports |
| [plans/](plans/README.md) | Cartes et plans à ajouter, suivi des sources |
| [sessions/](sessions/README.md) | Modèle de journal des parties, décisions et inventaires |
| [voix/](voix/README.md) | Descriptions vocales et aperçus audio |
| [histoires/](histoires/README.md) | Textes et narrations produits par le studio NPC |
| [exports/](exports/README.md) | Futurs PDF et aides de jeu imprimables |
| [archives/](archives/README.md) | Livret d’origine conservé intégralement comme archive figée |

## Faire évoluer la campagne

Modifier les fichiers de la zone concernée et les fichiers communs : ce sont les sources éditoriales de référence. L’archive d’origine ne reçoit pas ces modifications. Les références conservées aux chapitres du livret sont expliquées dans le [sommaire](campagne/README.md).

Lire [AGENTS.md](AGENTS.md) pour les contraintes et conventions. Décrire chaque évolution dans un commit et consigner les changements importants dans [CHANGELOG.md](CHANGELOG.md). Une branche et une pull request peuvent servir pour une révision à relire.

Les conversations ne sont pas synchronisées automatiquement avec GitHub. Reporter les décisions utiles dans les fichiers. Aucun plan graphique, calque ajusté ou export PDF n’est inclus dans cet import initial.

Ce dépôt contient les solutions et secrets du MJ. Préparer des documents distincts pour les joueurs ; les dossiers ne constituent pas des droits d’accès séparés.

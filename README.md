# CampagneBaston — La Compagnie des Huit Catastrophes

**À la recherche du laboratoire introuvable** : une campagne de fantasy comique pour **4 à 8 adolescents**, avec des profils maison pour **Chroniques Oubliées Fantasy 2**.

## Jouer et préparer

1. Lire la [mission](campagne/Mission.md), la [présentation](campagne/Presentation.md) et les [règles communes](campagne/Regles.md).
2. Laisser les joueurs choisir parmi les [huit zones](zones/README.md).
3. Préparer les [trois indices](indices/Indices.md) et la [conclusion au laboratoire](campagne/Final.md).
4. Pour jouer les PNJ, utiliser les [consignes communes](adventure.md), les fiches individuelles dans `characters/` et le `lore.md` de la zone.

**Retrouver le laboratoire de Malépine suffit à accomplir la quête.** Trois scénarios quelconques donnent les mêmes trois documents, dans l’ordre : **8 positions, puis 4, puis 1**. Le mage propose les destinations et aide à lire les supports.

Chaque scène locale tient en moins d’une heure. Elle présente un objectif concret, une action directe, un combat court possible et une solution sans combat. Un seul interlocuteur suffit pour comprendre quoi faire. Les êtres parlants et les enchantements font partie du monde ; aucune collecte magique annexe n’est nécessaire.

## Les huit destinations

| Destination | Environnement | Scénario |
| --- | --- | --- |
| Valombre | Grande ville | [retrait refusé, troll énervé](zones/grande-ville/Scenario.md) |
| Tilverton | Village | [la révolte des poules de Tilverton](zones/village/Scenario.md) |
| Cormanthor | Forêt | [le chêne a les glands](zones/foret/Scenario.md) |
| Le Grand Marais | Marécage | [le gué du crapaud-buffle](zones/marecage/Scenario.md) |
| L’Échine du Dragon | Montagne | [atchoum, vous êtes cuits](zones/montagne/Scenario.md) |
| La Sembie | Plaine | [la grève des hommes de paille](zones/plaine/Scenario.md) |
| L’Anauroch | Désert | [l’oasis qui prend la fuite](zones/desert/Scenario.md) |
| La côte de la Mer de Lune | Plage | [le trésor passe à la pince](zones/plage/Scenario.md) |

## Fichiers de jeu

La racine est utilisable directement dans NPC, sans import. Les fichiers sont modifiés sur place :

| Fichier | Contenu |
| --- | --- |
| `config.toml` | Langue, modèles et voix |
| [adventure.md](adventure.md) | Consignes communes des dialogues |
| `zones/<zone>/Scenario.md` | Objectif, action, combat, sortie express et document |
| `zones/<zone>/characters/*.md` | 33 fiches individuelles, dont Malépine dans la zone commune |
| `zones/<zone>/lore.md` | Décor public observable |
| `zones/<zone>/Monstres.md` | Profils chiffrés et conditions de fin des combats |
| `zones/<zone>/Objets.md`, lorsqu’il est présent | Équipement, prix, usages et charges |

Le catalogue de la plaine n’est pas présent ; sa récompense documentée figure dans la [fiche de Gaspard](zones/plaine/characters/gaspard.md#objets-associés--effets-exacts).

Les scénarios complets, solutions des indices et informations du MJ ne doivent pas être ajoutés au lore partagé.

## Préparation et suivi

- [Sommaire de campagne](campagne/README.md) et [aide du MJ](campagne/Aide-MJ.md).
- [Malépine](zones/commun/characters/archibald.md) et son [contexte public](zones/commun/lore.md).
- [Bestiaire général](zones/commun/Monstres.md) et [objets généralistes](zones/commun/Objets.md).
- [Plans](plans/README.md), [sélection](plans/SELECTION.md) et [sources des ressources](plans/SOURCES.md).
- [Voix](voix/README.md), [histoires](histoires/README.md) et [exports](exports/README.md).
- [Historique des évolutions](CHANGELOG.md).

Les cartes citées et les trois supports physiques demandent encore une préparation ; ne pas supposer qu’une image ou un calque ajusté est fourni. Les journaux décrivent une partie particulière et restent distincts du scénario de référence.

Ce dépôt contient des informations du MJ. Préparer des documents distincts pour les joueurs ; les dossiers ne constituent pas des droits d’accès séparés.

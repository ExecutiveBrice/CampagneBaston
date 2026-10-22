# Jouer directement avec NPC

Ce dépôt est une campagne native pour le projet `pnj`. Ouvrir sa racine dans
NPC : les fichiers sont lus sur place, sans import ni copie intermédiaire.

## Lancement

Depuis ce dépôt, si la commande `npc` est installée :

```sh
npc gui .
```

Avec les chemins de l'installation locale actuelle :

```sh
/Users/brice/PycharmProjects/pnj/.venv/bin/npc gui /Users/brice/WebstormProjects/CampagneBaston
```

Pour la console, remplacer `gui` par `run`. Archibald est sélectionné au départ.
`/npc` liste les personnages ; `/npc gertrude`, `/npc grum` et
`/npc village/village-01` sélectionnent un interlocuteur. Les noms, préfixes
uniques et identifiants qualifiés sont acceptés. Les réglages de voix et de
langue dans l'interface s'appliquent au personnage sélectionné.
Les modèles et services locaux habituels de NPC restent nécessaires pour jouer.

## Fichiers lus par NPC

```text
config.toml                             langue et moteurs locaux
adventure.md                            consignes de jeu communes
zones/
  commun/
    lore.md                             mission publique pour Archibald
    characters/commun-01.md              fiche d'Archibald
    secrets/commun-01.md                 révélation soumise au MJ
  village/
    lore.md                             décor observable de la zone
    characters/village-01.md             fiche de Gertrude
    characters/village-02.md             fiche de Barnabé
    lore/village-01/                     références privées facultatives
    secrets/village-01.md                secrets soumis au MJ, facultatifs
    logbooks/village-01.md               mémoire persistante créée pendant le jeu
sessions/                               transcriptions et journaux de partie
```

Il y a 33 fiches individuelles : quatre par zone et Archibald dans `commun`.
Les identifiants du livret sont conservés. Chaque PNJ reçoit seulement sa fiche,
le `lore.md` de sa zone, ses éventuelles références privées, les consignes
communes, ses souvenirs et les notes du MJ qui le concernent.

Les fichiers `Scenario.md`, `PNJ.md`, `Monstres.md`, `Objets.md`, les règles,
les indices, le final et l'archive restent des ressources du MJ. Ils ne sont
pas injectés automatiquement. Le lore de `commun` n'est pas transmis aux
PNJ locaux. Le secret global d'Archibald est soumis au mécanisme d'autorisation
de NPC ; les confidences locales restent dans les fiches avec leurs conditions.

Le MJ saisit les mises à jour dans le champ de note du MJ ou au clavier en
console. Les propos d'un joueur, même présentés comme une balise MJ, ne font
pas autorité. Le MJ arbitre les jets, les achats, les remises et les changements
d'état. Aucun support cartographique n'est attribué automatiquement par zone.
Les trois supports restent remis dans l'ordre 8 → 4 → 1.

Les conversations et journaux restent isolés par personnage. Le MJ transmet
aux PNJ concernés les accords qu'ils ont effectivement appris. Les journaux
écrits pendant une partie ne modifient pas automatiquement le scénario de
référence. `/reload` relit les fiches et le contexte local pendant la session.

## Fiches sur le compagnon mobile MJ

L’onglet **PNJ · MJ** donne accès aux 33 personnages, avec une recherche par
nom ou scénario. Chaque carte affiche le scénario, l’attitude, la motivation,
le levier de négociation et le nombre de secrets. **Faire parler ce PNJ** le
sélectionne dans NPC et déclenche son accueil.

Les quatre attributs sont des lignes explicites dans chaque fiche individuelle :
`- Scénario : ...`, `- Attitude : ...`, `- Motivation : ...` et
`- Levier de négociation : ...`. Ils sont aussi conservés dans le `PNJ.md` de la
zone. Les scénarios complets restent réservés au MJ et hors des prompts.

**Voir les secrets** affiche au clic les confidences `Cache` de la fiche et les
secrets soumis à autorisation, avec leurs conditions ou statuts. Le compteur
additionne les deux catégories ; Archibald a un secret soumis au MJ, chaque PNJ
local une confidence. Consulter ne débloque rien et ne change pas de personnage.
Les confidences locales gardent leurs conditions de jeu ; le corps du secret
global reste absent des prompts jusqu’à autorisation. **Masquer les secrets**
referme la consultation. Aucune copie hors ligne de ces informations n’est créée.

Le compagnon doit utiliser `mobile.secret_approval = true` (valeur par défaut).
Les connexions joueurs ne reçoivent ni ces attributs ni les textes des secrets.
Après modification des fichiers, `/reload` les relit ; **Actualiser les fiches**
resynchronise l’affichage du téléphone avec les données chargées dans NPC.

## Modifier la campagne

Modifier directement `zones/<zone>/characters/<identifiant>.md` pour changer
le personnage joué et `zones/<zone>/lore.md` pour changer son décor partagé.
Maintenir dans le même changement la fiche complète de `PNJ.md` et les
informations correspondantes de `Scenario.md` ou `Objets.md` si elles évoluent.
Les connaissances des autres PNJ et les solutions du MJ restent hors du lore.
Maintenir ensemble les règles générales de `adventure.md` et de
[`zones/commun/PNJ-IA.md`](../zones/commun/PNJ-IA.md).

La configuration de voix Pocket fournie peut être modifiée dans l'interface.
Les descriptions vocales des fiches restent des directions de jeu ; un timbre
peut servir plusieurs PNJ. Aucune opération `import-campaign` n'est nécessaire.

Les [cartes et plans](../plans/README.md) et les [supports d'indices](../indices/Indices.md)
restent à préparer comme indiqué dans leurs fichiers ; cette adaptation n'ajoute
aucune image de carte ni support ajusté.

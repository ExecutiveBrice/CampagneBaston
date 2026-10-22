# Voix de la campagne

Les descriptions et aperçus de `conteur` et `troll` proviennent de l'ancien dossier
`tools/voice_design/` du projet NPC. Chaque TOML contient le texte de démonstration,
la description de voix `instruct` et la langue. Le WAV voisin est son aperçu.

Pour générer un aperçu, avec l'option Qwen installée :

```sh
/Users/brice/PycharmProjects/pnj/.venv/bin/npc voice-design /Users/brice/WebstormProjects/CampagneBaston/voix/conteur.toml
```

Ajouter `--force` pour remplacer un WAV déjà présent. Le studio mobile enregistre
également ses nouveaux profils ici : un JSON et un WAV par identifiant.
Les WAV sont conservés localement et ignorés par Git.

Les [histoires](../histoires/README.md) sont rangées à part. Les descriptions et
aperçus ne sont pas injectés dans les prompts des personnages.

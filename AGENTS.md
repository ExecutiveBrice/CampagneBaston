# Instructions de travail — CampagneBaston

## Source et périmètre

- Lire le README, le sommaire de `campagne/` et les fichiers concernés avant une modification.
- Sources éditoriales canoniques : les quatre fichiers `Scenario.md`, `PNJ.md`, `Monstres.md`, `Objets.md` de chaque dossier `zones/<zone>/`, ainsi que les fichiers de `campagne/`, `commun/` et `indices/`. Modifier le fichier correspondant au sujet.
- `archives/La_Compagnie_des_Huit_Catastrophes.md` est l’original figé de l’import initial : ne pas le mettre à jour avec les évolutions. Aucun livret consolidé automatiquement n’est fourni.
- Chaque zone doit conserver ses quatre fichiers complets ; les catégories PNJ, Monstres et Objets ne sont pas de simples liens vers le scénario. Les règles et ressources généralistes sont partagées dans les dossiers communs.
- Les journaux dans `sessions/` décrivent une partie particulière ; ils ne changent pas automatiquement le scénario de référence.
- Garder les identifiants des PNJ, des objets OBJ/GEN et des rencontres REN stables. Si un titre change, réparer ses liens dans les index.
- Ne pas supposer qu’un plan, une image ou un outil externe est disponible parce qu’il est cité dans une conversation. Consulter les ressources effectivement présentes.

## Contraintes de la campagne

- Écrire en français, pour 4 à 8 adolescents, avec une fantasy comique originale évoquant l’esprit de Naheulbeuk : situations absurdes, institutions ridicules et personnages de mauvaise foi.
- Chaque zone doit rester jouable en moins d’une heure. Conserver les solutions sociales, les sorties express et la place de chacun dans un grand groupe.
- Huit environnements libres : grande ville, village, forêt, marécage, montagne, plaine, désert, plage.
- Trois scénarios, quels qu’ils soient, permettent de terminer la mission. Les mêmes trois supports cartographiques sont remis successivement par le MJ, sans association obligatoire à une zone.
- Progression des indices : huit possibilités, puis quatre (le deuxième indice doit en laisser plus de deux), puis une seule. Ne jamais bloquer un indice essentiel derrière un jet ou un achat.
- Les éclats résolvent les anomalies locales ; ils n’ouvrent pas automatiquement un portail. Les documents identifient l’entrée du laboratoire.
- Maintenir environ quatre PNJ par zone et distinguer leurs connaissances locales des secrets du MJ. Les instructions IA restent indépendantes d’un outil ou d’un moteur vocal précis, sauf demande explicite d’intégration.
- Garder les secrets globaux hors des consignes d’un PNJ qui les ignore. Le MJ décide des actions, achats, jets et changements d’état.

## Règles et matériel

- Base actuelle : Chroniques Oubliées Fantasy 2, profils maison pour héros débutants ; ne pas présenter ces chiffres comme les profils officiels.
- Pour les créatures : conserver DEF, PV, initiative, caractéristiques, attaques, armes, DM, armures, capacités, tactiques, moral et butin. Adapter l’effectif au groupe et la durée à une courte scène.
- Ne pas mélanger PV et variante express dans le même combat.
- Pour chaque objet : préciser nature, effet de base, bonus éventuel, pouvoir éventuel, limites/charges, prix et classe ou usage pertinent. Un objet peut être utile sans bonus ni magie. Éviter les doubles comptages et le cumul non prévu.
- Distinguer les 20 PO de frais communs des 30 PO par héros promis à la fin.
- L’humour vise les situations et les personnages ; conserver le ton adapté aux adolescents défini dans le livret.

## Vérification et livraison

- Préserver le contenu sans rapport avec la demande et tenir les index à jour.
- Vérifier les chemins et ancres Markdown touchés ; vérifier les calculs ou codes modifiés. Pour les indices, contrôler le passage 8 → 4 → 1.
- Signaler honnêtement les cartes absentes et les supports encore à fabriquer. Conserver l’origine et les conditions de réutilisation connues des ressources importées dans `plans/SOURCES.md`.
- Mettre à jour `CHANGELOG.md` pour les évolutions significatives. Les exports sont des produits dérivés datés, à régénérer depuis les sources.
- Respecter le fonctionnement de contribution demandé dans la session ; une pull request n’est pas une obligation systématique.

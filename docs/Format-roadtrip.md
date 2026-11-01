# Format Tour de France

Ce document décrit comment le contenu du roadtrip est écrit pour des **adultes slovaquophones** qui apprennent le français, du niveau débutant (après l'introduction et le kit de survie) jusqu'à un **bon A2, avec des incursions vers le B1**. Il reprend le format du roadtrip du cours sk-fr (`docs/Format-roadtrip.md` dans [Slovingo-sk-fr](https://github.com/lstux/slovingo-sk-fr)) et indique ce qui s'inverse. L'histoire, les personnages et l'itinéraire sont dans `Concept-adulte.md` ; la progression dans `Progression-roadtrip.md`.

La base reste le **SMD (Slovingo Markdown)** : voir `docs/Format-SMD.txt` dans le repo [Slovingo](https://github.com/lstux/Slovingo/tree/main/docs).

## Ce qui s'inverse par rapport à sk-fr

| | sk-fr (roadtrip) | fr-sk (tour de France) |
|---|---|---|
| Langue apprise | slovaque | **français** |
| Langue des explications | français | **slovaque** |
| « Toi » (`[USER_NAME]`) | Gab, le Français | **Andrea**, la Slovaque (formes **féminines**) |
| Guide | Andrea | **Gab** |
| Parcours | Bratislava → Košice | **Lyon → Saint-Marc-sur-Mer** |
| Narrateur | la navigation, en slovaque | la navigation, **en français** |
| Enfants | Hugo, Lola (Français) | Hugo, Lola (Français) **et Samo (Slovaque)** |
| Gag de registre | le *vy* de Gab | le **vous** d'Andrea |
| Heures, jours, nombres | les nombres slovaques | les nombres français (*soixante-dix, quatre-vingts*) |

Ce qui ne change pas : une série = un chapitre ; 6 fiches par série ; micro-dialogues dans les fiches 01 à 04 ; l'épisode dans les fiches 05 et 06 ; une photo par fiche ; une carte du trajet dans la fiche 01 ; le ton décalé et tendre.

## 1. Ton et rédaction

- Phrases courtes, répliques vives. L'humour vient des situations de voyage (la valise, la pause pipi, le ronfleur, « on est arrivés ? »), jamais d'une moquerie sur des personnes réelles.
- Ton d'adulte : second degré, autodérision de Gab, étonnements d'Andrea, logique implacable des enfants.
- Une idée à la fois, pas de jargon grammatical dans le texte (« partitif », « imparfait »…) avant que la fiche l'ait expliqué en quelques mots simples.
- Le guide touristique passe par les personnages : Gab raconte, les enfants demandent, la navigation annonce. Pas de paragraphe encyclopédique dans les dialogues ; les faits détaillés vont dans le **coin français**.
- Le français est celui d'un natif, naturel, **sans calque du slovaque**. Le slovaque des explications est à faire relire par un locuteur natif.

## 2. Une série = 6 fiches = un chapitre = un lieu

- **Fiches 01 à 04** : apprentissage (vocabulaire, un point de grammaire) avec des **micro-dialogues** qui font avancer la journée : route, visite, repas, arrivée au logement.
- **Fiche 05** : première partie de l'épisode (dialogue).
- **Fiche 06 (« extra »)** : tableau complet du vocabulaire **et** suite de l'épisode, qui se termine en général par **la nuit** (le logement du soir).

Un chapitre peut couvrir deux ou trois jours de voyage (Paris, Saint-Marc). La narration le signale (*Le lendemain…*), sans que la structure change.

## 3. Personnages, avatars et prénom

Le moteur associe **un nom par emoji** pour tout le cours, et les voix se règlent par emoji. **Chaque personnage a donc un marqueur unique.** Un marqueur peut combiner deux emojis, à condition de ne contenir aucune lettre.

| Avatar | Personnage | Notes |
|---|---|---|
| 🐰 | **Andrea** (toi) | `[USER_NAME]`, par défaut *Andrea* ; formes **féminines** (*je suis allée, contente, fatiguée*) |
| 🦊 | **Gab** | Français, guide, formes **masculines** |
| 🧢 | **Hugo** | renardeau, 9 ans, neveu de Gab *(avatar et âge proposés)* |
| 🐇 | **Lola** | petite hase, 6 ans, nièce de Gab *(avatar et âge proposés)* |
| 🎒 | **Samo** | petit lièvre gris, 8 ans, neveu d'Andrea *(avatar et âge proposés)* |
| 📱 / 🐰🌴 | **Claire** | sœur de Gab : voix au téléphone (📱), et en vrai à Nice puis à Saint-Marc (🐰🌴, à tester dans le moteur) |
| 🦊⚓ / 🦊🧶 | **Michel** et **Martine** | les parents de Gab, chapitre 12 *(avatars proposés)* |
| 🧭 | **La navigation** (le GPS) | narratrice par défaut, voir §6 |
| 💬 | Le narrateur neutre | repli, voir §6 |
| 🧑‍… | Les humains | désignés par leur **fonction**, un emoji par fonction (voir ci-dessous) |

**Humains** : ils parlent normalement aux animaux et personne ne s'en étonne. Un même emoji ne peut pas servir à deux fonctions (le moteur leur donnerait le même nom). Propositions : 🧑‍💼 la réception, 🧑‍🍳 le serveur, 🧓 l'hôte du gîte, 🧑‍🏫 le guide, 🧑‍🔧 le gardien du camping, 🧑‍🦰 la vendeuse, 👵 une vieille dame, 👷 le préposé de la remontée. On complète la liste au fil de l'écriture et on la tient à jour ici.

**Tutoiement et vouvoiement** :
- *tu* entre Andrea, Gab et les enfants, et en famille (chez Claire, chez Michel et Martine) ;
- **exception voulue : le *vous* d'Andrea envers Gab** (voir `Concept-adulte.md`). Chaque réplique où Andrea vouvoie Gab porte une remarque `+` qui le signale, pour que l'apprenant ne prenne pas cette forme pour la bonne ;
- *vous* avec tous les adultes inconnus (réception, serveurs, guides) ; les enfants vouvoient aussi les adultes qu'ils ne connaissent pas ;
- la navigation vouvoie le conducteur (*Tournez à droite*), comme une vraie navigation.

**Prénom** :
- `[ASK_USER_NAME]` est dans la première fiche de l'introduction, une seule fois. Ensuite, `[USER_NAME]` dans les répliques et la narration.
- Le nom par défaut (`site.user_name_default` dans `lang.json`) est *Andrea*. Le prénom n'est jamais écrit en dur dans les remarques : toujours `[USER_NAME]`, ou la 2e personne (« tvoja chyba »). Pas de `[USER_NAME]` dans une voix `{{…}}`.
- Dans le kit (souvenir de Villeurbanne), toi et Gab vous présentez au vouvoiement.
- Le marqueur va **après** le `!` : `! 🐰 Bonjour !`.

## 4. Genre

- Gab est un homme : formes masculines (*je suis parti, content*). Andrea et Lola : féminines (*je suis partie, contente*). Hugo et Samo : masculines.
- Le cours est écrit pour une apprenante (Andrea) : les accords au féminin des participes sont donc un sujet permanent, présenté dans les fiches de passé composé.
- La navigation se dit **la navigation** (féminin) et parle au féminin quand elle parle d'elle-même (*Je recalcule l'itinéraire*).

## 5. Écouter plutôt que lire

- **`{{…}}` contient du français et seulement du français** : le moteur le lit à voix haute avec la voix française. **Jamais de slovaque dans `{{…}}`** : le TTS le lirait de travers (c'était une erreur du Kit de survie de l'ancienne version).
- Les explications en slovaque ne sont pas lues ; le slovaque s'écrit en texte normal.
- Les **noms de lieux** du voyage (*Lyon, Chamonix, Pontrieux*) peuvent être en `{{…}}` : ce sont des mots français.
- Pas de `**gras**` dans un `{{…}}`.
- Les tableaux de vocabulaire ont l'en-tête **`Francúzština | Slovenčina`** (français en premier) : la colonne « parlable » est détectée par ce nom. Les tableaux de prononciation (voir l'introduction) mettent les exemples français en `{{…}}`.

## 6. La navigation 🧭 et le narrateur neutre 💬

La navigation parle un français net, lent, en **phrases très courtes**, et **vouvoie** Gab :

```
! 🧭 Dans deux cents mètres, tournez à droite.
> O dvesto metrov odbočte doprava.
> Dans deux cents mètres = o dvesto metrov
> tournez = odbočte
> à droite = doprava
```

Règles :
- phrases **très courtes**, au **présent** tant que le passé n'est pas introduit ;
- ses formules (*tournez, continuez tout droit, recalcul de l'itinéraire, votre destination est à droite*) s'apprennent d'abord **en bloc**, avant que l'impératif soit expliqué (chapitre 06) ;
- **elle n'est pas toujours là** : sans réseau (camping de Chamonix, Pontrieux, chez Claire), elle l'annonce (*Signal perdu*), se tait ou boude, puis revient avec *Recalcul de l'itinéraire…* ;
- quand une scène a besoin d'être située sans elle, on prend le **narrateur neutre 💬** ; on peut aussi basculer toute la série sur lui si la navigation s'essouffle ;
- les deux apparaissent dans `## Postavy` quand ils parlent dans la fiche.

## 7. Structure des fichiers

```
md/
├── 00_Introduction_NN_titre.md        (4 fiches, relues)
├── 10_Series_00_KitSurvie_NN_titre.md (à réécrire : souvenir de Villeurbanne)
├── 10_Series_NN_Etape_YY_titre.md     (roadtrip : séries 01 à 12)
├── 20_Vocabulary_NN_titre.md          (inchangé)
└── 99_Merci_01_Merci_01_merci-sk.md   (inchangé)
exercises/   un fichier .exercises.json par fiche
img/         photos et img/credits.md
docs/        concept, format, progression, histoire, planche de personnages
```

Exemple : `10_Series_02_Camargue_01_les-flamants.md`.

- **Titres** : `# Séria Camargue (1/5) — Les flamants` ; extra : `# Camargue (extra) — La nuit au gîte`.
- Le **thème** du nom de fichier donne la clé de `lang.json` → `subgroups`, `subgroup_themes` et les icônes de carte, en minuscules et **sans diacritiques** (voir `Progression-roadtrip.md`). Dans `lang.json`, les clés de `subgroups` sont **les clés nues** (`lyon`, `nice`…), pas `series_lyon`, avec le libellé en slovaque (`"paris": "Paríž"`).
- Noms de fichiers sans accent ; titres avec.
- **Exercices** : on les écrit à la main, mais il faut vérifier dans le moteur où ils sont lus (le build lisait `md/<fiche>.exercises.json`, pas `exercises/`). À tester dès la première série avant d'en écrire beaucoup.

## 8. Vocabulaire

- **Fiche d'apprentissage** : **7 à 8 mots** essentiels dans les chapitres 1 à 3 (on part de zéro), puis **9 à 10** ; plus 3 mots complémentaires. Un mot déjà vu (introduction, kit, chapitre précédent) reste dans le tableau, sans marque, et il est cité sous le tableau dans une ligne `Déjà vus, à revoir : {{…}}, {{…}}.`
- **Fiche 05** : au plus **5 mots « à retenir »**, signalés : `+ Nové slovo: {{…}} = …`. Les autres mots inconnus de la scène sont simplement expliqués dans la décomposition (`>`), sans être à retenir.
- **Fiche 06** : au plus **3 mots à retenir**, signalés et ajoutés au tableau récapitulatif ; le reste, comme dans la 05, par la décomposition.
- Au plus **une** forme « à écouter » (pas encore apprise) par fiche de dialogue, signalée par `+ Na počúvanie: …`. Les formules de la navigation comptent comme des blocs à retenir.
- Aucun mot inconnu sans explication, navigation et narrateur compris.
- Les noms de lieux ne comptent pas comme mots nouveaux.
- Les points de grammaire (accords, partitif, passé composé) sont donnés en **morceaux à retenir** (*un peu de, du fromage, je suis allée*), sans théorie.

## 9. Fiche d'apprentissage (01 à 04)

```markdown
# Séria Camargue (1/5) — Les flamants

@ TODO_img/nom.jpg | TODO : choisir une photo (…) sur Wikimedia Commons

(fiche 01 seulement : la carte du jour, voir ci-dessous)

Courte intro en slovaque (1 à 2 phrases) qui situe la journée.

---

## Nové slová
| Francúzština | Slovenčina |
|--------------|------------|
| … | … |

Déjà vus, à revoir : {{…}}, {{…}}.

---

## Dnešná gramatika
### Un point de grammaire
Explication en quelques phrases, tableau d'exemples.

---

## Dialóg
(micro-dialogue de 3 à 6 répliques avec avatars, navigation comprise)

---

## Francúzsky kútik
2 courts paragraphes sur le lieu du jour, mots-clés en {{…}}

---

## Doplnková slovná zásoba
(3 mots)

---

## Ešte pár viet
(2 cartes qui réutilisent les mots complémentaires)
```

**La carte du jour** : la fiche 01 de chaque série commence, juste après le titre et l'image, par une **carte Leaflet du trajet de la journée** (bloc `%~`, points numérotés dans l'ordre) ; les fiches suivantes peuvent ajouter une carte d'épingles (`%:`) pour les lieux visités. Coordonnées à régler avec `tools/geomap-editor.html` du moteur ; syntaxe dans `docs/Format-SMD.txt`, §5.

```
%~ Jour 1 : de Lyon à Villeurbanne
% 45.7640, 4.8357 | {{Lyon}}
% 45.7676, 4.8801 | {{Villeurbanne}}
```

*(Coordonnées de l'exemple approximatives.)*

Les micro-dialogues font **3 à 5 répliques au début du voyage, jusqu'à 8 vers la fin**. La section `## Dialóg` ne contient que des cartes avec avatar : le moteur la reconnaît comme dialogue.

## 10. Fiches 05 et 06 : l'épisode

**Fiche 05** :
- `## Slovná zásoba dialógu` (au plus 5 mots nouveaux) ;
- `## Postavy` : avatar + nom (`- 🧭 Navigation`, `- 🧢 Hugo`…) ;
- `## Dialóg` : l'épisode, une **scène entière**, écrite d'un trait comme dans `docs/Histoire.md`, **12 à 15 répliques** au chapitre 1, **15 à 20** jusqu'au chapitre 4, puis jusqu'à **30–40** vers la fin ;
- Coin français.

**Fiche 06 (extra)** :
- `## Všetka slovná zásoba série` : le tableau complet ;
- `## Postavy` ;
- `## Pokračovanie` : la suite et la fin de la journée, souvent **la nuit au logement** ; même longueur que la 05 ; **3 mots nouveaux au maximum**, signalés ; les exercices ne portent que sur les répliques sans mot nouveau ;
- Coin français.

## 11. Cartes audio

```
! 🦊 Combien ça coûte ?
> Koľko to stojí?
> Combien = koľko
> ça = to
> coûte = stojí
+ Remarque utile.
```

- La phrase après `!` est en **français** (c'est ce qui est lu).
- Première ligne `>` : traduction **slovaque** naturelle ; lignes suivantes : décomposition **une ligne par élément**, jamais plusieurs éléments séparés par des points-virgules.
- Lignes `+` : remarque, mot nouveau, astuce, ou signalement d'un *vous* d'Andrea.
- Dialogues : `! 🐰 Bonjour !` (avatar après le `!`).
- Typographie française : espace avant `? ! : ;`.

## 12. Photos

```
@ https://commons.wikimedia.org/wiki/Special:FilePath/<Fichier>.jpg | <sujet> — <auteur>, <licence>, Wikimedia Commons
```

- **Photos réelles** des lieux du voyage, une par fiche, sur Wikimedia Commons. Chaque photo a sa ligne dans `img/credits.md` (fiche, fichier, auteur, licence).
- Quand une photo ne montre pas exactement le lieu de la scène, la légende le dit.
- Tant que l'auteur n'est pas relevé, la légende finit par « crédit à compléter, Wikimedia Commons ».
- Mise en place, depuis la racine du cours : `tools/fill_credits.py` (s'il existe dans ce repo, sinon celui de sk-fr), puis `fetch_images.py` du moteur. Les deux vont **lentement** pour éviter les erreurs 429.
- Pas d'illustrations de personnages pour l'instant ; la planche `docs/illustrations/planche-personnages.jpg` sert de référence.

## 13. Coin français

Court, **vérifiable** (pas de chiffre approximatif), relié au **lieu du jour** : une date, une légende, une spécialité, un usage, un mot. C'est la partie « guide » du cours. Les faits sont vérifiés sur des sources sérieuses (sites officiels, offices de tourisme, UNESCO). Les **lieux touristiques réels** sont nommés ; pas de marque de produit ni de personnalité réelle dans les dialogues.

Les erreurs de fait repérées dans l'ancienne version (coutumes slaves présentées comme françaises, WC « réunis » en France, cidre pris pour du *mušt*…) sont à éviter : chaque affirmation sur « les Français » doit être vérifiée.

## 14. Qualité de langue

- **Français** : naturel, adulte, sans calque du slovaque.
- **Slovaque** : celui qu'un adulte slovaque dirait, sans tchèquisme. À faire relire.
- **Pièges slovaque → français** :

| ❌ | ✅ |
|----|----|
| Je suis une infirmière. | Je suis infirmière. (pas d'article après *être* pour un métier) |
| Je veux un café. (sec) | Je voudrais un café. |
| J'ai allé à Nice. | Je suis allée à Nice. |
| Je suis peur. | J'ai peur. |
| Je mange pas du pain. | Je ne mange pas de pain. |
| Je vais à la France. | Je vais en France. |
| Plus bon | Meilleur |

## 15. Exercices faits main

Écrits à la main dans `exercises/<nom de la fiche>.exercises.json` (voir §7 pour la vérification de l'emplacement), avec `"mode": "replace"` et `"sync": "full"` ; que du déjà vu ; une seule bonne réponse ; distracteurs qui ciblent les vraies confusions d'un slovaquophone (*le / la, un / une, du / de la, avoir / être au passé composé*) ; les 5 types quand la fiche s'y prête ; `[USER_NAME]` n'est jamais un trou ni une réponse. Les répliques de la navigation et du narrateur peuvent servir à l'écoute, mais ni de trou ni de réponse piège.

## 16. Vérifier avant de publier

- [ ] Photo choisie (ou TODO explicite), crédits dans `img/credits.md`
- [ ] Fiche 01 : carte du trajet du jour
- [ ] 7-8 (ch. 1-3) ou 9-10 nouveaux mots + 3 complémentaires ; 5 au plus en 05, 3 au plus en 06
- [ ] Cartes décomposées une ligne par élément
- [ ] Aucun mot inconnu sans explication, navigation et narrateur compris
- [ ] Aucun slovaque dans `{{…}}`
- [ ] Un marqueur unique par personnage, `! 🐰 …` après le `!`
- [ ] Formes féminines pour Andrea, Lola et la navigation ; masculines pour Gab, Hugo et Samo
- [ ] *tu / vous* respectés ; tout *vous* d'Andrea envers Gab est signalé par un `+`
- [ ] Coin français : faits vérifiés sur le lieu du jour
- [ ] Fiche extra : tableau complet, suite de l'épisode, 3 mots nouveaux au plus
- [ ] Nom de fichier et titre selon le schéma, sous-groupe déclaré dans `lang.json`
- [ ] Slovaque relu par un locuteur natif
- [ ] Ton : décalé, tendre, jamais cynique

Build local (depuis le repo [Slovingo](https://github.com/lstux/Slovingo)) :

```
python3 src/build.py --lang-dir ../slovingo-fr-sk --static-dir static
```

Après une modification de fiche, relancer `python3 src/sync_exercises.py --lang-dir ../slovingo-fr-sk`.

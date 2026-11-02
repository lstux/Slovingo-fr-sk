# Illustrations IA du Tour de France — prompts Gemini

Prompts pour la **planche de personnages n° 2** (les nouveaux personnages) et pour la **couverture** (image d'introduction). Les illustrations de scène (une par chapitre, pour la fiche 05) viendront plus tard, sur le modèle de `Prompts-illustrations.md` du repo sk-fr.

**Style** : illustration 2D dessinée à la main, personnages animaux, décors peints réalistes pour que les lieux soient reconnaissables. On dit « livre illustré original », pas « film d'animation » : Gemini a refusé une formulation « film » pour le kit de sk-fr (« intérêts de fournisseurs de contenu tiers »).

## Méthode

1. **La planche n° 1 est reprise telle quelle** : `docs/illustrations/planche-personnages.jpg` (Eric, Andrea, Hugo, Lola ; dans sk-fr, Eric s'appelle Gab). Rien à regénérer.
2. **Planche n° 2** : joindre la planche n° 1, coller le prompt « Planche n° 2 ». Garder la meilleure, la ranger dans `docs/illustrations/planche-personnages-2.jpg`.
3. **Couverture** : joindre **les deux planches**, coller le prompt « Couverture ». Pas de photo de référence.
4. Si un personnage dérive (couleurs, vêtements, oreille d'Andrea), le redemander en citant la planche : « keep the characters exactly as in the model sheets ».
5. Déposer l'image dans `img/illus_cover.jpg` (1920×1080, ou réduite à 1280 px de large).

**Crédit** : « Illustration générée avec Google Gemini ». Pas de photo de référence, donc pas de crédit Commons.

## Les personnages

| | Personnage | Description à garder |
|---|---|---|
| 🦊 | Eric | renard roux, la quarantaine, pointes d'oreilles gris foncé, quelques poils gris aux joues ; sweat zippé bleu, T-shirt blanc, sac à dos aux bretelles jaunes |
| 🐰 | Andrea | hase grise, la quarantaine, bande blanche du front au museau, oreille gauche tombante (à droite sur l'image de référence) ; haut vert menthe |
| 🧢 | Hugo | renardeau, 9 ans ; casquette rouge, T-shirt rayé (chapitres 3 et 12) |
| 🐇 | Lola | petite hase, 6 ans, fourrure sable clair, pas de bande blanche ; robe jaune (chapitres 3 et 12) |
| 🎒 | Samo | petit lièvre gris, 8 ans, neveu d'Andrea : même gris et même bande blanche qu'elle, **deux oreilles dressées**, sac à dos rouge ; **proportions d'enfant** (grosse tête ronde, jambes courtes, arrive à la taille d'un adulte) |
| 🐰🌴 | Claire | **lapine** adulte, fourrure beige sable, oreilles dressées, plus lapine que hase pour la distinguer d'Andrea ; sœur d'Eric, mère de Hugo et Lola ; lunettes de soleil relevées entre les oreilles, chemise blanche, jean clair (retenue sur la planche n° 2, v1) |
| 🦊⚓ | Michel | renard âgé, fourrure orange passée, museau gris, pull marine, casquette plate (retenu sur la planche n° 2, v1) |
| 🦊🧶 | Martine | renarde âgée **de taille adulte** (la tête arrive au menton de Michel), vrai museau de renard, oreilles pointues à pointes grises, fourrure abricot, joues argentées, lunettes rondes sur une chaînette, gilet vert d'eau |

---

## Planche n° 2 — la famille

À joindre : la planche n° 1.

```
Use the attached model sheet as the style and design reference. It shows four characters: an adult red fox, an adult grey hare with a white blaze, a fox cub in a red cap and a little sandy-brown hare in a yellow dress. Keep exactly that drawing style, line quality, proportions and colour palette.

Create a second model sheet for an original illustrated book, on a plain light background, with four new characters standing side by side at the same scale, each shown front view and three-quarter view, full body, with a few facial expressions (smiling, surprised, amused):

1. Samo, an 8-year-old male grey hare, the nephew of the adult grey hare on the attached sheet: same grey fur and white blaze from forehead to nose, so the family resemblance is obvious, but both his ears stand straight up (the tip of one slightly bent), big curious eyes, a small gap between his front teeth. He wears a navy T-shirt with a small mountain print, khaki shorts, sneakers and a red school backpack.
2. Claire, an adult female hare in her late thirties, light sandy-brown fur with a white tummy (the same colours as the little sandy-brown hare on the attached sheet, who is her daughter), long ears, a warm, slightly harried, amused look, sunglasses pushed up between her ears. She wears a white linen shirt and light jeans. She is the sister of the adult red fox.
3. Michel, an elderly male red fox in his early seventies, the father of the adult red fox: faded orange fur, grey muzzle and white eyebrows, grey-black ear tips, a slightly round belly, kind weathered face. He wears a navy knitted sweater and a flat cap.
4. Martine, an elderly female red fox in her late sixties, the mother of the adult red fox: soft apricot-orange fur, silvery cheeks, grey-black ear tips, round glasses on a chain, a big warm smile. She wears a sea-green cardigan over a flowery blouse.

Height: Claire about the same height as the adult grey hare on the attached sheet; Michel about the height of the adult red fox, a bit wider; Martine slightly shorter than Michel; Samo reaches the adult grey hare's chest.

Style: hand-drawn 2D illustration for an original illustrated book (not 3D, not pixel art): clean ink outlines, flat colours with soft cel shading, expressive faces. Warm, gentle summer light. Anthropomorphic animals walk upright, wear clothes and live among ordinary humans, who are drawn in the same 2D style and find this normal. No text, no letters, no speech bubbles, no logos, no watermark.
```

### Retour sur la v1 (1er novembre) et passe 2

La v1 est gardée dans `docs/illustrations/planche-personnages-2_v1.jpg`. **Retenus** : Claire (plus lapine que hase, ce qui la distingue d'Andrea) et Michel. **À refaire** : Samo, trop grand pour 8 ans (proportions d'ado), et Martine, ratée (taille d'enfant, visages de lapine au lieu de renarde).

À joindre : la v1 **puis** la planche n° 1.

```
Use the first attached image (the second model sheet, version 1) and the second attached image (the first model sheet) as references. Redraw the second model sheet in exactly the same style, background and layout, with these changes.

KEEP exactly as drawn: Claire (the beige rabbit with sunglasses, white shirt and light jeans) and Michel (the elderly fox in the navy sweater and flat cap), including their size, colours and expressions.

REDRAW Samo, the 8-year-old grey hare: he is a small CHILD, not a teenager. Child proportions: large round head (about one quarter of his body height), short arms and legs, a rounder belly, big eyes. His full height, ears excluded, reaches only Claire's waist, about 60% of Michel's height. Same grey fur and white blaze from forehead to nose, both ears up, navy T-shirt with a small mountain print, khaki shorts, sneakers, and a smaller, child-sized red school backpack.

REDRAW Martine, Michel's wife, an elderly red fox in her late sixties, as an ADULT nearly as tall as Michel (her head reaches his chin), softly plump, standing upright. She is clearly a FOX, not a hare and not a child: pointed muzzle with a cream chin and a black nose, upright pointed ears with grey-black tips, apricot-orange fur with silvery cheeks, a bushy tail with a cream tip. Round glasses on a chain around her neck, a sea-green cardigan over a flowery blouse, a long skirt, a big warm smile. Her face views (front, three-quarter, laughing) must be fox faces with a muzzle, never rabbit faces.

Height order, tallest first: Claire (ears included) and Michel, then Martine, then Samo.

Style: hand-drawn 2D illustration for an original illustrated book, clean ink outlines, flat colours, soft cel shading, plain light background, front view and three-quarter view for each character plus a few facial expressions. No text, no letters, no speech bubbles, no logos, no watermark.
```

### Retour sur la v2 (1er novembre) et passe 3

La v2 est gardée dans `docs/illustrations/planche-personnages-2_v2.jpg`. **Retenus** : les visages et les tenues de Martine (de vraies têtes de renarde), Claire, Michel, la tête de Samo. **À corriger** : l'échelle. Gemini tire chaque personnage vers la même hauteur : Samo est encore trop grand et Martine encore trop petite. On ne touche donc qu'aux proportions, avec une ligne de sol commune et des repères de hauteur.

À joindre : la v2 seulement.

```
Use the attached model sheet as the exact reference. Keep EVERYTHING the same: the same four characters, faces, expression heads, clothes, colours, drawing style and layout. Change ONLY the scale of the four full-body figures, which must stand on one common ground line, shown as a height line-up, with very faint thin horizontal guide lines (no text, no numbers, no labels) at the height of the top of Michel's cap, of his chest, and of his belt.

Heights, with the top of Michel's flat cap = 100%:
- Michel, the elderly fox with the cap: 100%.
- Claire, the beige rabbit: her head (ears excluded) reaches 95% of Michel's height; her long ears go above him.
- Martine, the elderly fox in the green cardigan: 90%. She is an adult, only slightly shorter than Michel: the tips of her ears reach the top of Michel's cap, her head reaches his chin. Bigger than she is now.
- Samo, the 8-year-old grey hare: 62%. His head (ears excluded) reaches only Michel's chest and Claire's waist. Smaller than he is now. Keep his child proportions: a large round head, short arms and legs, a small red backpack.

Keep the face and expression heads as drawn, only redistribute them around the line-up. Plain light background, no text, no letters, no logos, no watermark.
```

### Planche n° 2 retenue (v3, 1er novembre)

Les échelles sont bonnes. La planche retenue est `docs/illustrations/planche-personnages-2.jpg` : la v3 de Gemini, **sans les repères de hauteur ni leurs étiquettes, et sans la colonne de visages de droite**, retirés par script. Ordre : Michel, Claire (avec ses deux têtes d'esquisse), Martine, Samo. À joindre avec la planche n° 1 pour la couverture et les scènes.

**Si Gemini dérive encore** (Martine surtout) : la faire seule, puis l'assembler à la main avec le reste.

```
Use the attached model sheet (Michel, the elderly fox in the navy sweater) as the style and design reference, and the first model sheet for the overall drawing style.

Single-character model sheet, plain light background: Martine, Michel's wife, an elderly ADULT red fox in her late sixties, nearly as tall as Michel (her head reaches his chin), softly plump. A fox, with a pointed muzzle, a cream chin and a black nose, upright pointed ears with grey-black tips, apricot-orange fur with silvery cheeks, a bushy tail with a cream tip. Round glasses on a chain, a sea-green cardigan over a flowery blouse, a long skirt, a big warm smile. Show her full body in front view and three-quarter view, plus three fox-face expressions (smiling, laughing, surprised). Same style as the references: hand-drawn 2D illustration for an original illustrated book, clean ink outlines, flat colours, soft cel shading. No text, no letters, no logos, no watermark.
```

---

## Couverture — l'image d'intro (retenue le 1er novembre)

Image : `img/illus_cover.jpg` (1280 px de large), branchée sur la page de choix du cours (`site.cover` dans `lang.json`). Elle servira aussi à la fiche d'introduction « Le voyage », quand elle sera écrite.

Composition retenue : Lyon et la basilique de Fourvière au pied des Alpes à gauche, la campagne au centre, Paris (tour Eiffel, Sacré-Cœur) à l'horizon, Mont-Saint-Michel et la mer à droite ; la voiture est de face, volant à gauche, Eric conduit, Andrea tient la carte, Samo est derrière. Il a fallu plusieurs essais : les prompts trop chargés mélangeaient les lieux (flamants, deux Lyon).

À joindre : les deux planches. Pas de photo de référence.

```
Use the two attached model sheets for the characters: keep them exactly as designed (first sheet: the adult red fox and the adult grey hare; second sheet: Samo, the small grey hare child on the far right).

Create a wide panoramic illustration, 16:9 landscape (1920×1080), for the cover of an original illustrated book about a family road trip across France.

FOREGROUND (lower centre): a small, slightly dusty light-blue family car with a roof box full of luggage, seen from the FRONT in a three-quarter view, driving towards the viewer on a winding country road. It is a French car with the steering wheel on the LEFT side of the car. Because we see the car from the front, the driver therefore sits on the RIGHT side of the picture. The driver is the adult red fox, both paws on the wheel, smiling but a little tired. Next to him, in the front passenger seat on the left of the picture, sits the adult grey hare, holding an unfolded paper road map, amused. In the back seat, between them, Samo the small grey hare child leans forward with wide, amazed eyes, his red backpack on his lap. All three faces are clearly visible through the windscreen. The car takes up about a quarter of the image height.

LEFT SIDE (background and middle ground): big snowy Alpine mountains. At their foot, one single city: Lyon, with the white Basilica of Notre-Dame de Fourvière on its hill, terracotta rooftops, and the Rhône and Saône rivers with a few bridges.

CENTRE (far background, on the horizon): Paris, with the Eiffel Tower and the white-domed Sacré-Cœur on its hill, small and light in the haze.

RIGHT SIDE (background): the tidal island of Mont-Saint-Michel with its Gothic abbey rising from the sand, and beyond it the blue sea with a beach, a lighthouse and two or three sailboats.

BETWEEN THEM: peaceful green rolling countryside with fields, a vineyard and a few small villages with church steeples. The winding road leads from the car back across the countryside towards the horizon. The bottom-right area of the image is just countryside and road, with no city and no buildings except one or two small farmhouses.

Leave a calm strip of sky across the top (a few summer clouds) for a title.

Do NOT include: flamingos, horses, lavender fields, cable cars, a second copy of any city, or any other landmark.

Characters: Eric, an adult male red fox in his forties (bright orange fur, grey-black ear tips, cream muzzle and chest, a few grey hairs on the cheeks, friendly slightly tired eyes), wearing a blue zip hoodie over a white T-shirt; Andrea, an adult female grey hare in her forties (grey fur, a white blaze from forehead to muzzle, long ears with pink insides, her left ear folded down, calm amused look), wearing a mint-green top; Samo, an 8-year-old male grey hare (same grey fur and white blaze as Andrea, both ears standing up, big curious eyes), in a navy T-shirt with a small mountain print, drawn with small child proportions (large round head, short body).

Style: hand-drawn 2D illustration for an original illustrated book (not 3D, not pixel art): clean ink outlines, flat colours with soft cel shading, expressive faces, detailed realistic painted backdrops true to the real landmarks. Warm, gentle summer light. Anthropomorphic animals walk upright and wear clothes. No text, no letters, no speech bubbles, no logos, no watermark.
```

**Crédit** : « Illustration générée avec Google Gemini ». Détail connu : l'oreille tombante d'Andrea n'est pas visible dans l'habitacle.

---

## 01. Lyon — Fourvière

Fiche : `md/10_Series_01_Lyon_05_fourviere.md` → image `img/illus_01.jpg`

**À joindre** : la planche n° 1, la planche n° 2, et la photo de référence : [Lyon vu depuis la Basilique Notre-Dame de Fourvières.jpg](https://commons.wikimedia.org/wiki/File:Lyon_vu_depuis_la_Basilique_Notre-Dame_de_Fourvi%C3%A8res.jpg) (Celeda, CC BY-SA 4.0), déjà dans `img/` sous le nom `Lyon_vu_depuis_la_Basilique_Notre-Dame_de_Fourvieres.jpg`.

```
Use the attached model sheets for the characters (keep them exactly as designed): the first sheet for the adult red fox and the adult grey hare, the second sheet for Samo, the small grey hare child. Use the attached photo as the reference for the place: the view of Lyon from the Fourvière hill, with the Saône river and a red footbridge in the lower part, the old city with its orange roofs, and tall modern towers in the far distance, under a light summer haze.

Scene: A hand-drawn illustration for an original illustrated book. On the terrace of Fourvière above the city of Lyon, late morning in summer. In the lower left of the picture, seen from slightly behind in three-quarter view, the three travellers stand at a stone railing and look down at the city. The adult red fox, Eric, stretches one arm toward the view like a proud guide, with a big smile. Next to him, the adult grey hare, Andrea, amused and a little tired, rests one hand on the shoulder of Samo. The small grey hare child, Samo, on tiptoe, with his red backpack, points with wide eyes at the two rivers far below. The whole city of Lyon fills the rest of the picture, faithful to the reference photo. Leave the upper area fairly calm.

Characters: Eric, an adult male red fox in his forties (bright orange fur, grey-black ear tips, cream muzzle and chest, a few grey hairs on the cheeks, friendly slightly tired eyes), wearing a blue zip hoodie over a white T-shirt; Andrea, an adult female grey hare in her forties (grey fur, a white blaze from forehead to muzzle, long ears with pink insides, her left ear folded down, calm amused look), wearing a mint-green top; Samo, an 8-year-old male grey hare (same grey fur and white blaze as Andrea, both ears standing up, big curious eyes), in a navy T-shirt with a small mountain print and a red backpack, drawn with small child proportions (large round head, short body).

Style: hand-drawn 2D illustration for an original illustrated book (not 3D, not pixel art): clean ink outlines, flat colours with soft cel shading, expressive faces. Detailed realistic painted background faithful to the reference photo. Warm, gentle summer light. 16:9 landscape, 1920×1080. Anthropomorphic animals walk upright and wear clothes. No text, no letters, no speech bubbles, no logos, no watermark.
```

**Crédit** : « Illustration générée avec Google Gemini, d'après une photo de Celeda (Wikimedia Commons, CC BY-SA 4.0) ». Une illustration faite d'après une photo CC BY-SA en est une œuvre dérivée : elle reste sous CC BY-SA 4.0, avec le nom du photographe (voir `img/credits.md`).

---

## 02. Camargue — Le gîte

Fiche : `md/10_Series_02_Camargue_05_le-gite.md` → image `img/illus_02.jpg`

**À joindre** : la planche n° 1, la planche n° 2, et la photo de référence : [51 Mas camarguais réhabilité.jpg](https://commons.wikimedia.org/wiki/File:51_Mas_camarguais_r%C3%A9habilit%C3%A9.jpg) (Deuxtroy, CC BY-SA 3.0), déjà dans `img/` sous le nom `Mas_camarguais_rehabilite.jpg`.

```
Use the attached model sheets for the characters (keep them exactly as designed): the first sheet for the adult red fox and the adult grey hare, the second sheet for Samo, the small grey hare child. Use the attached photo as the reference for the place: a low traditional Camargue house with a thick reed-thatch roof and white-painted gable ends, a hedge in front, trees behind.

Scene: A hand-drawn illustration for an original illustrated book. Evening in the Camargue, golden light, a few rose-coloured clouds. The little light-blue car with its roof box is parked in front of the thatched house, in the fields; in the distance, a white horse and a few pink flamingos in a pond. At the door of the house an elderly human host in a cardigan hands the key to the adult red fox, Eric, who thanks him with a tired smile and holds a small bag. The adult grey hare, Andrea, stands behind him, tired, her travel bag on her shoulder, a hand on her back. The small grey hare child, Samo, already runs towards the door, red backpack bouncing, arms in the air. Ordinary humans are drawn in the same 2D style and find the animals completely normal.

Characters: Eric, an adult male red fox in his forties (bright orange fur, grey-black ear tips, cream muzzle and chest, a few grey hairs on the cheeks, friendly slightly tired eyes), wearing a blue zip hoodie over a white T-shirt; Andrea, an adult female grey hare in her forties (grey fur, a white blaze from forehead to muzzle, long ears with pink insides, her left ear folded down, calm amused look), wearing a mint-green top; Samo, an 8-year-old male grey hare (same grey fur and white blaze as Andrea, both ears standing up, big curious eyes), in a navy T-shirt with a small mountain print and a red backpack, drawn with small child proportions (large round head, short body).

Style: hand-drawn 2D illustration for an original illustrated book (not 3D, not pixel art): clean ink outlines, flat colours with soft cel shading, expressive faces. Detailed realistic painted background faithful to the reference photo. Warm, gentle evening light. 16:9 landscape, 1920×1080. No text, no letters, no speech bubbles, no logos, no watermark.
```

**Crédit** : « Illustration générée avec Google Gemini, d'après une photo de Deuxtroy (Wikimedia Commons, CC BY-SA 3.0) » ; elle reste sous CC BY-SA 3.0 avec le nom du photographe.

---

## Ensuite

Une illustration par chapitre pour la fiche 05, sur le même principe : planches jointes, photo de référence du lieu (lien Commons), prompt complet par scène. À préparer quand l'histoire sera écrite et relue.

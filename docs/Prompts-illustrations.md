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

**Si Gemini dérive encore** (Martine surtout) : la faire seule, puis l'assembler à la main avec le reste.

```
Use the attached model sheet (Michel, the elderly fox in the navy sweater) as the style and design reference, and the first model sheet for the overall drawing style.

Single-character model sheet, plain light background: Martine, Michel's wife, an elderly ADULT red fox in her late sixties, nearly as tall as Michel (her head reaches his chin), softly plump. A fox, with a pointed muzzle, a cream chin and a black nose, upright pointed ears with grey-black tips, apricot-orange fur with silvery cheeks, a bushy tail with a cream tip. Round glasses on a chain, a sea-green cardigan over a flowery blouse, a long skirt, a big warm smile. Show her full body in front view and three-quarter view, plus three fox-face expressions (smiling, laughing, surprised). Same style as the references: hand-drawn 2D illustration for an original illustrated book, clean ink outlines, flat colours, soft cel shading. No text, no letters, no logos, no watermark.
```

---

## Couverture — l'image d'intro

Pour l'introduction (`md/00_Introduction_01_francuzsko.md`) → image `img/illus_cover.jpg`.

À joindre : les deux planches.

```
Use the attached model sheets for the characters (keep them exactly as designed).

Scene: Opening image of a family road-trip story across France. A small, slightly dusty light-blue car with a roof box drives along a winding country road through a patchwork of French summer landscapes, seen from slightly above and in front. The adult red fox is driving, smiling but already a little tired; next to him the adult grey hare sits holding an unfolded paper road map, amused; in the back seat, the small grey hare Samo leans out of the open window with wide, amazed eyes, his red backpack on his lap. Behind them, the road winds past, from the foreground to the horizon: a vineyard and lavender fields, a pond with pink flamingos and white horses, snowy Alpine peaks on the left, the Eiffel Tower small in the distance, a rocky island topped by a Gothic abbey (Mont-Saint-Michel) rising from the sand, and on the far right a blue sea with a lighthouse. Leave the upper third of the image fairly calm (sky with a few summer clouds), as a title may be added later.

Characters: Eric, an adult male red fox in his forties (bright orange fur, grey-black ear tips, cream muzzle and chest, a few grey hairs on the cheeks, friendly slightly tired eyes), wearing a blue zip hoodie over a white T-shirt; Andrea, an adult female grey hare in her forties (grey fur, a white blaze from forehead to muzzle, long ears with pink insides, her left ear folded down, calm amused look), wearing a mint-green top; Samo, an 8-year-old male grey hare, her nephew (same grey fur and white blaze, both ears standing up, big curious eyes), in a navy T-shirt and a red backpack, drawn with small child proportions (large round head, short body).

Style: hand-drawn 2D illustration for an original illustrated book (not 3D, not pixel art): clean ink outlines, flat colours with soft cel shading, expressive faces. Backgrounds are detailed, realistic painted backdrops, true to the real landscapes and landmarks of France, arranged as a storybook collage along the road. Warm, gentle summer light. 16:9 landscape, 1920×1080. Anthropomorphic animals walk upright, wear clothes and live among ordinary humans, who are drawn in the same 2D style and find this normal. No text, no letters, no speech bubbles, no logos, no watermark.
```

---

## Ensuite

Une illustration par chapitre pour la fiche 05, sur le même principe : planches jointes, photo de référence du lieu (lien Commons), prompt complet par scène. À préparer quand l'histoire sera écrite et relue.

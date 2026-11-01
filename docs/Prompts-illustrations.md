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
| 🎒 | Samo | petit lièvre gris, 8 ans, neveu d'Andrea : même gris et même bande blanche qu'elle, **deux oreilles dressées**, sac à dos rouge |
| 🐰🌴 | Claire | hase adulte, fourrure sable clair comme Lola, sœur d'Eric, mère de Hugo et Lola ; lunettes de soleil relevées entre les oreilles |
| 🦊⚓ | Michel | renard âgé, fourrure orange passée, museau gris, pull marine, casquette plate |
| 🦊🧶 | Martine | renarde âgée, fourrure abricot, joues argentées, lunettes rondes sur une chaînette, gilet vert d'eau |

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

---

## Couverture — l'image d'intro

Pour l'introduction (`md/00_Introduction_01_francuzsko.md`) → image `img/illus_cover.jpg`.

À joindre : les deux planches.

```
Use the attached model sheets for the characters (keep them exactly as designed).

Scene: Opening image of a family road-trip story across France. A small, slightly dusty light-blue car with a roof box drives along a winding country road through a patchwork of French summer landscapes, seen from slightly above and in front. The adult red fox is driving, smiling but already a little tired; next to him the adult grey hare sits holding an unfolded paper road map, amused; in the back seat, the small grey hare Samo leans out of the open window with wide, amazed eyes, his red backpack on his lap. Behind them, the road winds past, from the foreground to the horizon: a vineyard and lavender fields, a pond with pink flamingos and white horses, snowy Alpine peaks on the left, the Eiffel Tower small in the distance, a rocky island topped by a Gothic abbey (Mont-Saint-Michel) rising from the sand, and on the far right a blue sea with a lighthouse. Leave the upper third of the image fairly calm (sky with a few summer clouds), as a title may be added later.

Characters: Eric, an adult male red fox in his forties (bright orange fur, grey-black ear tips, cream muzzle and chest, a few grey hairs on the cheeks, friendly slightly tired eyes), wearing a blue zip hoodie over a white T-shirt; Andrea, an adult female grey hare in her forties (grey fur, a white blaze from forehead to muzzle, long ears with pink insides, her left ear folded down, calm amused look), wearing a mint-green top; Samo, an 8-year-old male grey hare, her nephew (same grey fur and white blaze, both ears standing up, big curious eyes), in a navy T-shirt and a red backpack.

Style: hand-drawn 2D illustration for an original illustrated book (not 3D, not pixel art): clean ink outlines, flat colours with soft cel shading, expressive faces. Backgrounds are detailed, realistic painted backdrops, true to the real landscapes and landmarks of France, arranged as a storybook collage along the road. Warm, gentle summer light. 16:9 landscape, 1920×1080. Anthropomorphic animals walk upright, wear clothes and live among ordinary humans, who are drawn in the same 2D style and find this normal. No text, no letters, no speech bubbles, no logos, no watermark.
```

---

## Ensuite

Une illustration par chapitre pour la fiche 05, sur le même principe : planches jointes, photo de référence du lieu (lien Commons), prompt complet par scène. À préparer quand l'histoire sera écrite et relue.

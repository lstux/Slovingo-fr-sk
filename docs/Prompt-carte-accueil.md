# Fond de la carte d'accueil

Image à produire : `img/map_background.jpg`, portrait 9:16 (768 × 1376 ou 1080 × 1920), à générer avec Gemini à partir du prompt ci-dessous. Même principe que dans sk-fr (`docs/Prompt-carte-accueil.md` du repo Slovingo-sk-fr).

Le parcours va de haut en bas dans l'ordre des chapitres : Lyon en haut, Saint-Marc-sur-Mer en bas. La carte est **stylisée** : ce n'est pas la géographie exacte de la France (qui ferait un trajet en boucle, avec des étapes superposées), mais un voyage qui descend le long d'une seule route qui serpente. Les paysages changent peu à peu : le Sud et les Alpes, la Bourgogne, Paris, le Nord, la Normandie, la Bretagne, puis l'Atlantique. Pas de texte sur l'image, les libellés viennent de l'application.

Une fois l'image reçue :
1. la copier dans `img/map_background.jpg` et ajouter une ligne dans `img/credits.md` (illustration générée avec Gemini, prompt dans ce fichier) ;
2. régler les positions dans `lang.json` (`map.positions`, en % de l'image) et les icônes (`map.icons`) ; l'éditeur est `python3 ../Slovingo/tools/map_editor.py .` ;
3. étapes de la carte : intro, kit de survie, les 12 séries, puis la fiche finale `99_Credits_01_merci.md`.

## Prompt

```
Vertical illustrated travel map of France, 9:16 portrait (1080×1920), seen from a high bird's-eye angle. Detailed, warm digital painting, golden-hour light, soft and slightly muted colours so that small round markers placed on top stay readable. Same spirit as a vintage tourist poster map, but painterly and realistic, no cartoon.

A single winding road crosses the whole image from the top edge to the bottom edge, in a gentle zigzag (left, right, left…). The road trip goes from top to bottom. Along the road, in order, small vignette-sized landmarks, each in its own area, alternating left and right of the road. The scenery changes gradually from warm southern landscapes at the top to green northern and Atlantic landscapes at the bottom:

1. Top: the road enters from the top edge, coming from far away.
2. Lyon: the white basilica of Fourvière on its green hill above two rivers, red-tiled roofs, a small tram crossing a bridge.
3. The Camargue: flat marshland with white horses and pink flamingos, a low thatched farmhouse, the high medieval walls of Aigues-Mortes with a round tower in the distance.
4. The Côte d'Azur: a long curved promenade lined with palm trees along a turquoise sea, pebble beach, a few white yachts in a harbour, a market with striped awnings.
5. The Alps: tall snowy peaks, the Mont Blanc massif, a cable car, a green mountain meadow with a cow, a small blue lake with a little old town (Annecy-like) on its shore.
6. Dijon: a medieval town with a colourful glazed-tile roof, vineyards in rows on a gentle hillside.
7. Paris: the Eiffel Tower, the winding Seine with a stone bridge, grey zinc roofs.
8. Lille: a Flemish-style square of brick houses with stepped gables, a tall belfry, a hint of flat northern fields.
9. Étretat: white chalk cliffs with a natural stone arch above a grey-blue sea, a pebble beach.
10. Mont-Saint-Michel: the granite abbey rock rising from huge sandy tidal flats, a straight causeway, a few sheep on the salt meadows.
11. Brittany, the Trieux valley: a small river with a tidal estuary, a little railway line running along it, a harbour with boats, and an island with a lighthouse and pink granite rocks.
12. Angers: a dark fortress with round striped towers beside the Maine river, a vineyard and a tuffeau-stone château on the Loire.
13. Bottom: a sandy Atlantic beach with a small seaside town, a long promenade, wooden beach cabins and a few small sail boats, the road ending by the sea under a warm sunset.

Rolling green hills, forests, fields and rivers fill the space between landmarks. Keep the road and the areas right next to each landmark uncluttered.

No text, no letters, no labels, no signs, no flags, no logos, no map legend, no compass, no frame or border, no people in the foreground, no animal characters in clothes.
```

## Remarques pour les retouches

- Si Gemini fait un vrai plan de la France avec contour de côtes : insister sur « no country outline, no coastline map, one single continuous road from top to bottom ».
- Si les monuments sont trop petits ou trop serrés : redemander en précisant « each landmark takes about 8% of the image height ».
- À éviter : les drapeaux, les panneaux de villes, les cartes de randonnée (texte automatique).

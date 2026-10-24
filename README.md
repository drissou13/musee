# Musée DB Prod 13 — visite 3D

Un musée virtuel en HTML / CSS / JavaScript (three.js) : on se promène à la première personne dans sept salles de photos.

.

## Contrôles
- Flèches ou ZQSD : marcher
- Glisser la souris ou le doigt : regarder autour
- Clic ou toucher sur un tableau : l'afficher en grand
- Sur mobile : boutons ▲ ▼ ◀ ▶ à l'écran

## Ajouter ou changer des photos
1. Déposer l'image dans `photos/`.
2. Ajouter une ligne dans le tableau `PHOTOS` en haut du script de `index.html` :
   `{ "src": "photos/mon-image.jpg", "title": "Mon titre", "room": "Salle des Platines" }`
3. Garder les photos d'une même salle côte à côte dans le tableau, et mettre `"first": true` sur la première photo de chaque salle pour afficher la bannière.

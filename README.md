# Musée DB Prod 13 — visite 3D

Un musée virtuel en HTML / CSS / JavaScript (three.js) : on se promène à la première personne dans sept salles de photos.

## Voir le musée
- **GitHub Pages** : Settings → Pages → Branch `main` / dossier `/ (root)`. Le site sera disponible sur `https://drissou13.github.io/NOM-DU-DEPOT/`.
- **En local** : ouvrir un terminal dans le dossier puis lancer `python3 -m http.server`, et aller sur http://localhost:8000
  (ouvrir `index.html` directement par double-clic ne charge pas les photos à cause des règles du navigateur sur les textures WebGL).

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

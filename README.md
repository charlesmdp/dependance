# Dépendance du Moulin de Saint-Christophe en 3D

Maquette 3D interactive de la grange (dépendance) après rénovation, refaite à partir des plans APS au 1:50 et du devis de travaux.

Ce qu'on peut faire sur la page :

- Vues Extérieur, Étage, RDC (maison de poupée, sans toit), hauteur de coupe réglable.
- « Meubles entiers » : en vue RDC ou Étage, les murs sont coupés bas mais les meubles de l'étage restent entiers jusqu'à son plafond. « Toiture » enlève le toit, même sans coupe.
- Visite à pied à hauteur d'yeux (ZQSD ou flèches, souris ; E ou clic pour ouvrir les portes et les fenêtres, t'asseoir sur le canapé ou t'allonger sur les lits, L pour la lumière de la pièce).
- Fenêtres qui s'ouvrent : en visite, d'un clic dans les autres vues, ou toutes d'un coup avec « Fenêtres ouvertes ».
- Allumer et éteindre les lumières pièce par pièce, ambiance Jour ou Soir.
- Pompe à chaleur : chauffage, clim ou arrêt, split par split, avec les flux d'air visibles ou non. Les flux montrent aussi l'air chaud du poêle qui passe la grille vers la bergerie et l'aspiration de la VMC de la bergerie.
- Dehors : l'étang devant, le mur de berge, la cour en gravier, le garage aux portes vertes (non visitable) et le bûcher, placés d'après le site du moulin.

Le bouton (i) en haut à droite liste ce qui vient des plans, ce qui vient du devis et ce qui est supposé.

Le numéro de la version en ligne est écrit en haut du panneau (« Maquette V12 ») : s'il ne correspond pas à la dernière version, le site n'a pas été redéployé ou le navigateur garde l'ancienne page en cache.

## Fichiers

- `index.html` : toute la page en un seul fichier. three.js r147 est chargé depuis cdn.jsdelivr.net, les textures sont générées dans le navigateur.

Les plans et le devis ne sont pas dans ce dépôt : il est public et ces documents contiennent des coordonnées personnelles.

## Mise en ligne sur Cloudflare Pages

1. Cloudflare, Workers & Pages, Create, Pages, Connect to Git, choisir `charlesmdp/dependance`.
2. Framework preset : None. Build command : vide. Build output directory : `/`.
3. Save and Deploy. Chaque push sur `main` redéploie le site.

Pour tester en local : `python3 -m http.server` dans le dossier, puis ouvrir http://localhost:8000.

# Image Texte v2.0.0

Appli Android : **lire le texte de vos images** (une ou plusieurs à la fois, sans Internet) et **retoucher vos images**.

## Deux APK (même paquet `bf.alphamat.imagetexte`, même clé)
- `ImageTexte_v2.0.0.apk` : Android 8 et plus (décors animés, images de travail plus grandes).
- `ImageTexte_Lite_v2.0.0.apk` : Android 5.0 / 5.1 et plus (décors fixes, mémoire réduite).

⚠️ La v2 est une nouvelle appli (nouveau paquet, vraie clé de signature) : désinstallez l'ancienne « ImageTexte » 1.0.x avant.

## Fonctions
- **Lire** : photo ou choix de plusieurs images → texte lu à la suite, modifiable, copier / partager / enregistrer, « Retoucher et relire », tout réunir, export .txt. Partager › Image Texte depuis la galerie ou WhatsApp.
- **Textes** : bibliothèque avec recherche sans accents, vignette de l'original, renommer, export .txt.
- **Retouche** : rogner (Libre, Carré, 4:3, 3:4, 16:9, 9:16), pivoter, miroir, redresser au ½ degré, luminosité / contraste / saturation / chaleur, 12 filtres, textes (5 polices, couleur, contour, ombre, fond, déplacer / agrandir / tourner), dessin (pinceau, surligneur, ligne, flèche, cadre, cercle), Document (remettre une page à plat avec loupe, noir & blanc net, couleurs nettes, gris contrasté, plus net), Annuler / Rétablir, comparer avec l'original, enregistrer dans Images/ImageTexte, partager.
- 5 thèmes 3D animés, réglages en menus repliables, aide complète, « Mes autres applis et logiciels ».

## Technique
Java pur (aucune bibliothèque d'interface), lecture du texte par ML Kit (modèle latin intégré à l'APK).
Clé : `app/imagetexte.jks` (mot de passe `ImageTexte2026bf`, alias `imagetexte`) — à conserver pour toutes les mises à jour.
Compilation : déposer `ImageTexte_vX.Y.Z.zip` à la racine du dépôt ; GitHub Actions compile les deux APK et les publie dans Releases.

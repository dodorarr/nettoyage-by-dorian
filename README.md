# NETTOYAGE by DORIAN – site vitrine

Site d'une seule page (HTML/CSS/JS, sans dépendance), pensé pour le mobile et Google Ads.

## Modifier les prix, le téléphone, l'e-mail
Tout est en haut du `<script>` à la fin de `public/index.html`, dans le bloc « À MODIFIER FACILEMENT » :
`TARIFS`, `TRAITEMENT`, `MINIMUM`, `FORFAITS`, `TEL_WA`, `EMAIL`.
Le tableau des tarifs, l'estimateur et le formulaire se mettent à jour tout seuls.

## Ajouter des photos
Mettre les images dans `public/img/` (format `.webp` de préférence, environ 1200 px de large),
puis ajouter un bloc `<figure>` dans la section `#photos`.

## Google Ads
1. Dans Google Ads, créer une conversion « Contact » (clic sur le téléphone ou WhatsApp).
2. Coller la balise `gtag` fournie dans le `<head>` (emplacement indiqué en commentaire).
3. Renseigner `ADS_ID` et `CONV_CONTACT` dans le script.

## Mettre en ligne (Firebase Hosting)
```bash
npm install -g firebase-tools
firebase login
firebase use --add      # choisir le projet nettoyagebydorian
firebase deploy --only hosting
```

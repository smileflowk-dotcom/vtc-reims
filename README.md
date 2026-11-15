# VTC Reims — mini landing page

Une **mini-page unique** (un écran sur mobile 390 × 844 et sur ordinateur 1440 × 900) avec design noir/or, sans dépendance ni compilateur.

## Contenu

- Titre « Votre VTC à Reims sur réservation ».
- 3 lignes sur les trajets : gares de Reims et Champagne-Ardenne TGV, CDG/Orly, Reims–Épernay et alentours.
- **2 boutons compacts seulement** : « Appeler » (tel: +33 7 49 51 07 10) et « Envoyer un SMS » (application SMS ouverte avec message prérempli).
- Pas de long formulaire, pas de faux avis, pas de promesse de disponibilité immédiate.

## Vérifications locales

- Test Chromium : viewport mobile 390 × 844, petit mobile 320 × 700 et ordinateur 1440 × 900.
- **Aucun défilement**, aucun débordement horizontal, aucune erreur JavaScript dans ces tests.
- Les liens `tel:` et `sms:` ont le bon numéro ; la réception effective sur téléphone n'est pas encore testée.

## Avant publication commerciale

Le site reste volontairement en `noindex,nofollow` ; le nom commercial et les mentions légales du chauffeur doivent encore être confirmés. Le SMS n'envoie rien automatiquement et la course n'est confirmée qu'après accord du chauffeur.

Le code est conservé sur GitHub. GitHub Pages peut être inadapté à un site commercial de réservation au regard de ses conditions d'utilisation : vérifier les conditions d'hébergement avant activation.

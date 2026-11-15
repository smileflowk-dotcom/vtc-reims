# VTC Reims — landing page compacte

Site statique monopage pour un chauffeur privé VTC à Reims. **Version de préparation, non publiée sur un hébergement web.**

## Design

- Référence visuelle : page VTC CDG du dépôt `smileflowk-dotcom/vtc-reservation`.
- Nouvelle présentation sombre, or discret, centrée et mobile-first.
- **3 boutons d'action principaux au total** : appel dans l'en-tête de la page, préparation SMS dans le formulaire, appel discret fixe sur mobile.
- Boutons compacts (bouton principal d'environ 45 px de haut).
- Sans faux avis, fausse disponibilité immédiate, prix inventé, publicité ou scripts tiers.

## Données du chauffeur

- Numéro : **07 49 51 07 10** / `+33749510710`.
- Zones évoquées : Reims, Bezannes, Tinqueux, Cormontreuil, Épernay.
- Transferts à organiser : gares de Reims et Champagne-Ardenne TGV, CDG, Orly, déplacements professionnels.
- Nom commercial de l'entreprise **non communiqué** ; « VTC Reims » est pour l'instant un descriptif éditorial, pas une dénomination commerciale déclarée.

## Contact / formulaire

- Appel direct via liens `tel:`.
- Formulaire sans backend : collecte trajet, date, heure, passagers, bagages, nom, téléphone, précisions.
- Vérification navigateur des champs obligatoires et de la date.
- À validation, tentative d'ouverture d'un SMS prérempli vers `+33749510710`. Le client doit appuyer lui-même sur **Envoyer**.
- **Aucune réservation automatique et aucun envoi serveur** ; toute course doit être confirmée par le chauffeur.
- Les liens SMS ne sont pas universellement pris en charge sur ordinateur et restent à tester sur un vrai téléphone.

## Tests effectués

- HTML analysé : **3 boutons principaux**, bon numéro ; aucun ancien numéro parisien.
- Chromium Playwright : captures mobile 390 px / desktop 1440 px, aucun débordement horizontal, aucune erreur JavaScript initiale.
- Bouton appel dans le hero d'environ 45 px, contre 22 px de texte + 20 px de padding de chaque côté dans la référence.
- Champs du formulaire : validation des champs obligatoires testée ; données d'exemple acceptées.
- **À tester** : ouverture réelle de l'application SMS sur Android/iOS et réception du message par le chauffeur.

## Publication ultérieure

À compléter avant toute mise en ligne commerciale :

1. Confirmer le nom commercial réel, les mentions légales, le SIREN, l'identité juridique et les éventuelles informations réglementaires VTC nécessaires.
2. Vérifier prestations et horaires réels.
3. Tester l'envoi SMS et la prise de contact sur téléphone.
4. Retirer `noindex,nofollow` uniquement une fois le site prêt, avec une URL définitive et une politique de confidentialité complète.
5. Publier sur un hébergement adapté aux activités commerciales. **GitHub Pages n'a pas été activé** ; ses conditions de service comportent des restrictions sur les sites à vocation commerciale transactionnelle.

Le dépôt GitHub sert de source de vérité. Le site n'exige aucun build, framework ni service externe ; un hébergeur compatible peut servir directement le fichier `index.html`.

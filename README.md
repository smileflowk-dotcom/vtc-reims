# Mini-site VTC Reims — version de prépublication

Site statique **une seule page** pour un chauffeur VTC indépendant intervenant à Reims et dans la Marne.

## Ce qui est prêt

- Design bleu nuit et or, responsive, sans dépendance externe ni compilation.
- Appel direct au **07 49 51 07 10** (`tel:+33749510710`).
- Présentation des trajets Reims Centre, Champagne-Ardenne TGV, CDG, Orly et Épernay.
- Cartes de trajet qui préremplissent le formulaire.
- Formulaire qui **prépare un SMS** sur le téléphone du visiteur. Le visiteur doit ensuite appuyer sur *Envoyer* dans son application SMS.
- Copie du récapitulatif et lien SMS de secours.
- Menu mobile, liens d'ancrage, FAQ, mentions et confidentialité provisoires.
- Aucun paiement, aucun backend, aucun formulaire envoyé ou stocké par le site.

## Vérifications réalisées

- 46 liens internes/de contact recensés ; aucun lien d'ancrage cassé.
- Tests Chromium sur écran mobile 390 px et ordinateur 1440 px : pas de débordement horizontal ni erreur JavaScript.
- Menu mobile s'ouvre/se referme ; six trajets préremplissent le formulaire ; lien SMS créé avec le numéro correct.
- **Non testé** : réception réelle d'un SMS par le chauffeur et compatibilité sur les téléphones réels.

## Avant toute mise en ligne commerciale

1. Confirmer le **nom commercial réellement utilisé**, la dénomination légale, le SIREN, les coordonnées et les informations réglementaires à faire figurer dans les mentions légales.
2. Confirmer les prestations et l'éventuelle activation de WhatsApp ; le formulaire utilise pour l'instant **SMS**, plus universel.
3. Compléter et valider les **mentions légales** et la **politique de confidentialité**.
4. Retirer la balise `noindex,nofollow` uniquement quand le site sera juridiquement et commercialement prêt.
5. Ajouter l'URL canonique et mettre à jour les données structurées avec l'identité commerciale confirmée.
6. Vérifier appel/SMS sur un vrai téléphone et demander au chauffeur de confirmer un trajet test.
7. Remplacer, si souhaité, l'illustration graphique par des photographies authentiques du véhicule.

## Hébergement

Le code se trouve dans `index.html` : aucun build n'est nécessaire.

> ⚠️ **GitHub Pages : restriction d'usage.** La documentation GitHub Pages indique que l'hébergement gratuit ne doit pas être utilisé pour un site d'entreprise principalement destiné à faciliter des transactions commerciales. Ce dépôt sert donc de **source GitHub**, pas de déploiement GitHub Pages du site VTC de réservation.
>
> Documentation officielle : https://docs.github.com/fr/pages/getting-started-with-github-pages/github-pages-limits

Pour publier une fois les informations réglementaires confirmées, connecter ce dépôt à un hébergeur de sites statiques autorisant les sites commerciaux (par exemple Netlify, sous réserve de ses conditions en vigueur). Aucun build : publier le dossier racine du dépôt.

## Propriété et sécurité

Le dépôt appartient à `smileflowk-dotcom`. Le nom personnel du chauffeur n'apparaît pas dans le contenu commercial. La fiche Google Business Profile est un projet distinct ; aucune fiche n'a été créée ni modifiée.

# DUVARO — boutique de démonstration

Site e-commerce statique (HTML/CSS/JS, sans dépendance), hébergeable sur GitHub Pages.
Toutes les données (panier, comptes, commandes, avis, réglages) sont stockées dans le navigateur (localStorage) : c'est une **démo fonctionnelle**, pas une boutique de production.

## Mettre en ligne sur GitHub Pages
1. Remplacer `OWNER/REPO` dans `index.html` (balise canonical), `robots.txt` et `sitemap.xml`.
2. Pousser ce dossier sur la branche `main` du dépôt.
3. Dépôt > Settings > Pages > Source : *Deploy from a branch*, branche `main`, dossier `/ (root)`.

## À compléter avant toute vente réelle
- Informations légales : mentions légales, CGV, confidentialité (zones surlignées « À compléter »).
- Prix, stocks, frais et délais de livraison : modifiables dans l'Espace gérant (`#admin`).
- Paiement réel (ex. Stripe Checkout), back-office serveur, comptes sécurisés, envoi d'emails :
  nécessitent un backend (ex. Shopify, ou Next.js + base de données + Stripe).
- Le routage par `#ancres` limite le référencement page par page : pour un SEO complet, prévoir des URL réelles (un fichier par page ou un framework avec rendu serveur).

## Structure
- `index.html` : application complète
- `404.html` : page d'erreur GitHub Pages
- `img/` : visuels produits (WebP)

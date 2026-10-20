# Mettre Aura Scanner en ligne (gratuit, depuis le téléphone)

## 1. Héberger (GitHub Pages)
1. Compte gratuit sur github.com, puis nouveau dépôt public « aura ».
2. Navigateur en « version ordinateur ». Add file > Upload files : envoie tous les fichiers du dossier (index.html, sw.js, manifest.webmanifest, 2 icônes, privacy.html).
3. Settings > Pages > Branch : main > Save. Ton site : https://TONPSEUDO.github.io/aura/

## 2. Abonnement (Stripe)
1. dashboard.stripe.com : crée le compte (activation avec tes infos et IBAN).
2. Payment Links > Nouveau : produit « Aura Premium », prix récurrent (ex. 2,99 €/semaine).
3. Après le paiement > « Rediriger vers ton site » : https://TONPSEUDO.github.io/aura/?premium=TON_CODE
4. Dans index.html, remplace STRIPE_LINK (lien du Payment Link) et PREMIUM_CODE (TON_CODE, longue suite de lettres et chiffres).
Limite : le code peut être partagé. Suffisant pour tester, à sécuriser (webhook Stripe) si ça décolle.

## 3. Pub (AdSense)
Demande l'approbation sur adsense.google.com avec ton site (privacy.html obligatoire, un nom de domaine propre est souvent exigé). Une fois approuvé, colle son script dans index.html (repère « ADSENSE ») et remplace les cadres « Espace publicitaire » par tes blocs.

## 4. Installer sur l'écran d'accueil
iPhone : Safari > Partager > Sur l'écran d'accueil. Android : Chrome > menu > Installer l'application.

## 5. Avant d'encaisser
Complète privacy.html. Pour vendre en France, vérifie le statut à avoir (par ex. micro-entreprise) : je ne suis pas juriste.

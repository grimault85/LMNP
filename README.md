# Grand Livre LMNP

Petit outil de saisie mensuelle pour une location meublée (LMNP, régime réel).
Vous déposez vos documents (comptes rendus de gestion, avis d'assurance, échéanciers
de prêt, avis de taxe foncière) et l'application produit un tableau mois par mois
des recettes et charges courantes, exportable en CSV.

Conçu comme un **journal de saisie** qui alimente un logiciel comptable : les
amortissements et la déclaration se font ailleurs. Le « résultat » affiché est un
indicateur de gestion, **avant amortissements** — ce n'est pas le résultat fiscal.

## Confidentialité

Tout est traité **localement dans le navigateur**. Aucun document, aucun chiffre
n'est envoyé sur un serveur. Les bibliothèques de lecture PDF sont chargées depuis
un CDN public (une connexion internet est nécessaire à la première ouverture).

⚠️ **Ne committez jamais vos données** (PDF, sauvegardes `.json`, exports `.csv`) —
le fichier `.gitignore` les exclut par défaut. Ce dépôt ne contient que le code.

## Utilisation

- **En local** : ouvrez `index.html` dans votre navigateur.
- **En ligne (GitHub Pages)** : activez Pages sur la branche `main`, puis ouvrez
  l'URL fournie. La sauvegarde automatique et l'export fichier fonctionnent des deux façons.

## Fonctions

- Reconnaissance automatique des pièces (relevé Laforêt, avis MACIF, échéanciers PCAS/PTZ, taxe foncière)
- Montants lus **vérifiables et modifiables à la main**
- Assurance PNO affectée à la **période réelle** de chaque avis
- Factures à **qualifier** (déductible / récupérable locataire / à immobiliser)
- **Détection de doublons** (relevés, échéanciers, avis)
- Colonne **taxe foncière** (lissée ou imputée à un mois)
- **Sauvegarde locale automatique** + sauvegarde/restauration par fichier
- Export CSV (tableau mensuel et détail par pièce)

## Sauvegarde

L'application mémorise l'état dans le navigateur (localStorage). Pour une archive
durable et transportable, utilisez le bouton **« Sauvegarder dans un fichier »** et
conservez le `.json` généré en lieu sûr (hors du dépôt Git).

## Licence

Usage personnel.

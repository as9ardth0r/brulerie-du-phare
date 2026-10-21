# Brûlerie du Phare

**Une boutique e-commerce de démonstration, en une seule page, sans dépendance.**

Catalogue filtrable, fiches produits, panier persistant et tunnel de commande avec paiement simulé — le tout en HTML, CSS et JavaScript natif. Aucune bibliothèque, aucun serveur : le fichier s'ouvre tel quel dans un navigateur et se publie sur GitHub Pages.

👉 **Démo en ligne : https://as9ardth0r.github.io/brulerie-du-phare/**

> Marque fictive. Aucun paiement réel n'est effectué : le parcours de paiement est une simulation destinée à montrer l'interface et la logique côté client.

## Ce que montre ce projet

- **Catalogue** filtrable par catégorie (doux, corsés, décaféinés, matériel).
- **Panier** complet : ajout, quantités, retrait, sous-total, frais de port et seuil de livraison offerte, le tout recalculé en direct.
- **Persistance** : le panier est conservé dans le navigateur (`localStorage`) d'une visite à l'autre.
- **Tunnel de commande** : formulaire de livraison, validation des champs, écran de confirmation avec numéro de commande.
- **Thème clair / sombre** automatique (selon le système) et commutable, mémorisé.
- **Responsive** et accessible : navigation au clavier, libellés ARIA, cibles tactiles confortables, `prefers-reduced-motion` respecté.
- **Visuels en SVG** : aucun recours à une banque d'images, rien à télécharger.

## Lancer le projet

Aucune installation. Au choix :

```bash
# ouvrir directement le fichier
xdg-open index.html

# ou servir le dossier
python3 -m http.server 8000
```

Puis rendez-vous sur http://localhost:8000.

## Publier sur GitHub Pages

1. Déposez `index.html` à la racine du dépôt.
2. **Settings → Pages → Branch : `main` / `/ (root)` → Save.**
3. La boutique est en ligne à `https://<utilisateur>.github.io/<dépôt>/` après une minute.

## Pour aller en production

Cette démo est volontairement tout en front-end. Une vraie boutique ajouterait un serveur pour : le prix calculé côté serveur, le stock, le paiement réel (Stripe, PayPal, Mollie) et la confirmation par webhook signé. Ces briques sont justement l'objet d'un projet frère : **[Guichet](https://github.com/as9ardth0r/guichet)**, qui montre l'intégration sécurisée de plusieurs passerelles de paiement en PHP.

---

Projet de démonstration réalisé par [Joel Broutin](https://as9ardth0r.github.io/portfolio/), développeur web à Wimereux. Licence MIT.

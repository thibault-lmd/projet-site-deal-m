# projet-site-deal-m

Projet pour essayer de vendre un site internet a deal'm

## Contenu

| Fichier | Rôle |
| --- | --- |
| `index.html` | Le site complet, en un seul fichier (CSS, JS et images embarqués en base64). Il suffit de l'ouvrir dans un navigateur ou de le déposer sur un hébergeur. |
| `planche.png` | Photo source — les steaks sur la plancha. Utilisée dans « Trois salles, une cuisine ». |
| `burgergrosplan.png` | Photo source — gros plan sur les burgers empilés. Colonne de droite de la même section. |
| `burgermain.png` | Photo source — affiche « Best Burgers ». Section click &amp; collect, en bas de page. |

Les `.png` sont les originaux Instagram. `index.html` en embarque des versions
WebP redimensionnées (~100 Ko chacune) pour que la page reste légère.

## Dépendances externes

Le fichier est autonome pour les images, mais charge trois ressources en ligne :

- Google Fonts (Archivo, Instrument Sans, Courier Prime) ;
- Leaflet 1.9.4 (CSS + JS) pour les cartes des trois adresses ;
- les tuiles CARTO, avec repli sur OpenStreetMap puis sur un plan dessiné en CSS
  si le réseau ne répond pas.

Sans réseau, la page reste lisible : polices système, plans de repli, et toutes
les animations continuent de fonctionner.

## À faire avant mise en ligne

- Remplacer les vignettes des fiches produit (encore générées par IA) par de
  vraies photos ; le bandeau d'avertissement dans « La carte » le signale.
- Confirmer avec le restaurant les compositions marquées « à confirmer »
  (Truffle, Baos) et les horaires.

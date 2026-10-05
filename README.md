# Dashboard Climat Suisse

Dashboard interactif en un seul fichier HTML visualisant l'évolution du climat
en Suisse à partir des données ouvertes de
[MétéoSuisse](https://www.meteosuisse.admin.ch/climat.html) (réseau
climatologique de base NBCN, 29 stations).

## Fonctionnalités
- Carte de la Suisse zoomable : sélection d'une station par clic ou liste déroulante
- Séries annuelles : précipitations, ensoleillement, température moyenne, extrêmes Tmin/Tmax
- Jours tropicaux (Tmax ≥ 30 °C) et jours de gel (Tmin < 0 °C) par année
- Moyenne mobile, tendances linéaires, anomalies, corrélations, distributions journalières
- Affichage en lignes ou en colonnes, plein écran par graphique, export CSV
- Accessibilité : description textuelle dynamique de chaque graphique pour les
  lecteurs d'écran, tableau des données annuelles repliable, lien d'évitement,
  statut de chargement annoncé, focus clavier visible
- Séries indépendantes par variable : si une station n'a pas une grandeur
  (ex. précipitations à Jungfraujoch), les autres graphiques restent complets

Le journal détaillé des changements (V1a → V1c) est en commentaire au début de
`dashboard_climat.html`.

## Utilisation
Ouvrir `dashboard_climat.html` dans un navigateur. Si le chargement des
données est bloqué en `file://`, servir le dossier en local :
`python -m http.server 8000` puis ouvrir `http://localhost:8000/dashboard_climat.html`.

Aucune dépendance à installer (Plotly chargé via CDN).

Application développée avec Claude Opus 4.8 (Anthropic).

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

## Utilisation
Ouvrir `dashboard_climat.html` dans un navigateur. Si le chargement des
données est bloqué en `file://`, servir le dossier en local :
`python -m http.server 8000` puis ouvrir `http://localhost:8000/dashboard_climat_V1b.html`.

Aucune dépendance à installer (Plotly chargé via CDN).

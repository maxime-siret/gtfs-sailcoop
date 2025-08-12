# GTFS — SAILCOOP Glénan 2025 (Concarneau ⇄ Saint-Nicolas)

> Données GTFS publiques pour la liaison bateau SAILCOOP entre **Concarneau**, **Beg Meil** (certains jours) et **Saint-Nicolas (archipel des Glénan)**.

- **Période couverte** : 2025-04-01 → 2025-09-30 (AMJ, Juil-Août, Septembre)
- **Type de ligne** : `route_type=4` (ferry)
- **Accessibilité** : PMR **oui** (`wheelchair_accessible=1`, `wheelchair_boarding=1`)
- **Vélos** : **interdits** (`bikes_allowed=2`)
- **Billetterie** : `agency_fare_url` vers le module de réservation + `route_url` d’information
- **Shapes réalistes** : sorties de port et approche du chenal (pas de segments droits)

---

## 🔗 Téléchargement

- **Dernière version (stable)** : `<https://maxime-siret.github.io/gtfs-sailcoop/latest.zip>` en date du 12 août 2025
- **Rapport de validation** : disponible [ici]([url](https://gtfs-validator-results.mobilitydata.org/c47c9ac5-72ed-4354-b232-684cd1811434/report.html))

---

## 📁 Contenu du GTFS

Fichiers principaux :
- `agency.txt` — opérateur (inclut `agency_fare_url`)
- `stops.txt` — arrêts **CONCARNEAU**, **BEGMEIL**, **STNICOLAS** (coords WGS84)
- `routes.txt` — ligne GLN (`route_type=4`, `route_url`)
- `trips.txt` — voyages (avec `shape_id`, `wheelchair_accessible=1`, `bikes_allowed=2`)
- `stop_times.txt` — horaires
- `calendar.txt` / `calendar_dates.txt` — service par période/jour
- `shapes.txt` — **CCN_STN**, **STN_CCN**, **BEG_STN**, **STN_BEG** (distances cumulées en mètres)
- `feed_info.txt` — métadonnées de diffusion

Optionnel :
- `fare_attributes.txt` + `fare_rules.txt` — grilles tarifaires (A/R : Adulte, Jeune, Enfant, <4 ans)

---

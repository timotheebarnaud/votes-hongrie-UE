# La Hongrie, mouton noir de l'Union européenne ? Analyse des votes au Conseil de l'UE

*Analyse du comportement de vote de la Hongrie au Conseil de l'Union européenne depuis le retour au pouvoir de Viktor Orbán (2010), complétée par les données de vetos au Conseil européen.*

## Visualisations

1. [La Hongrie, championne de l'opposition au sein de l'UE](https://www.datawrapper.de/_/dbh8n/) — Classement des votes "contre" par pays
2. [Une nette accélération de l'opposition ces dernières années](https://www.datawrapper.de/_/8sNCj/) — Votes "contre" de la Hongrie par année
3. [La justice et l'environnement, les deux combats majeurs](https://public.flourish.studio/visualisation/28396073/) — Votes "contre" et abstentions par thématique
4. [La Hongrie, seule contre tous](https://www.datawrapper.de/_/dnqOP/) — Isolement dans les votes "contre"
5. [La Pologne, meilleure alliée de la Hongrie](https://www.datawrapper.de/_/fYtBk/) — Pays votant "contre" aux côtés de la Hongrie
6. [Le droit de veto, une arme sur-utilisée par la Hongrie au Conseil européen](https://public.flourish.studio/visualisation/28393946/) — Vetos par pays et par thématique

## Méthodologie

Les 1 723 résultats de vote sont récupérés par **scraping** du [registre public des votes](https://www.consilium.europa.eu/en/general-secretariat/corporate-policies/transparency/voting-results/) du Conseil de l'UE, à l'aide de **Selenium** (Chrome en mode debug pour contourner Cloudflare) et **BeautifulSoup**. Les données sur les vetos au Conseil européen proviennent du [EU Veto Tracker](https://michalovadek.github.io/eu-veto-tracker/) de Michal Ovádek (UCL, 2025).

**Distinction importante** : le Conseil de l'UE (votes législatifs, majorité qualifiée) et le Conseil européen (vetos, unanimité) sont deux institutions distinctes. Un vote "contre" au Conseil de l'UE ne bloque pas l'adoption d'un texte — il exprime une opposition politique. Un veto au Conseil européen bloque effectivement la décision.

Données au 06/04/2026.

## Organisation du dépôt

```
├── data/
│   ├── raw/            # CSV brut du scraping + dataset vetos Ovádek
│   └── clean/          # Exports pour les infographies
├── notebooks/
│   └── votes_hongrie_UE.ipynb
└── README.md
```

## Outils

Python (pandas, Selenium, BeautifulSoup) · Datawrapper · Flourish · Jupyter Notebook

---

Projet réalisé par **Timothée Barnaud**.

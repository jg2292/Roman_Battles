
# The Spatial Geography of Roman Warfare

### Battle Locations, Territorial Boundaries, Settlements, and Military Infrastructure

**Author:** John Grace  
**Institution:** Georgetown University  
**Course:** PPOL 6805 / DSAN 6750  
**Project Type:** GIS Final Project

---

## Project Overview

This project examines the spatial geography of Roman warfare by investigating the geographic distribution of recorded Roman battles and their relationships with settlement patterns, historical territorial boundaries, and specialized infrastructure.

Using georeferenced battle locations, historical Roman territorial reconstructions, and settlement data from the [Pleiades Gazetteer](https://pleiades.stoa.org/), the analysis applies spatial statistical methods and Monte Carlo simulations to evaluate whether Roman battles exhibit patterns beyond those expected under spatial randomness.

The project distinguishes between two classifications of conflict:

- **External Conflicts:** Military engagements involving Rome and external opponents.
- **Civil Conflicts:** Military engagements involving internal Roman political or military factions.

The analysis investigates four primary questions:

1. Do Roman battle locations exhibit significant spatial clustering relative to complete spatial randomness?
2. Does the geographic distribution of known settlements help explain the distribution of Roman battles?
3. Are Roman battles disproportionately located near the historical territorial boundaries of Roman control?
4. Do external and civil conflicts exhibit different spatial relationships with military and civic infrastructure?

The results suggest that settlement geography, territorial boundaries, and specialized infrastructure each provide different perspectives on the spatial distribution of Roman warfare. No single geographic model fully explains the observed patterns.

---

## Final Manuscript

The completed research manuscript is available through GitHub Pages:

**[View The Spatial Geography of Roman Warfare](https://YOUR-USERNAME.github.io/roman_battles/)**

The manuscript was created using Quarto and includes the project's research background, data sources, methodology, statistical results, visualizations, and conclusions.

The primary manuscript source is `index.qmd`.

---

## Repository Structure

The repository is organized around the data collection process, exploratory analysis, statistical modeling, and final manuscript.

| Directory / File | Description |
|---|---|
| `Datacollection/` | Data collection workflows and source datasets used to construct the Roman battle and geographic datasets. |
| `HypothesisTest.qmd` | Main analytical workflow containing the spatial statistical analyses and Monte Carlo simulations used in the project. |
| `HypothesisTest.ipynb` | Jupyter notebook associated with the analytical workflow. |
| `EDA/` | Exploratory data analysis and preliminary investigation of the project datasets. |
| `index.qmd` | Final Quarto manuscript containing the research paper. |
| `GIS_Manuscript.bib` | Bibliography containing the manuscript's academic references. |
| `chicago-17-no-url.csl` | Citation style file used to format references. |
| `visualization/` | Maps, charts, and other visual outputs generated during the analysis. |
| `images/` | Additional images used in the project. |
| `tables/` | Tables and supporting analytical outputs. |
| `assets/` | Supporting assets used by the manuscript and website. |
| `style.css` | Custom styling for the rendered manuscript. |
| `docs/` | Rendered HTML output published through GitHub Pages. |
| `_quarto.yml` | Quarto project configuration. |
| `_freeze/` | Cached computational outputs used by Quarto. |

---

## Data Sources

The project combines several sources of historical and geographic information.

### Roman Battle Records

Battle records were collected using Wikidata and subsequently reviewed to determine Roman involvement and classify each engagement as either an external conflict or civil conflict.

The final dataset contains **342 battle-location records representing 332 unique battles**.

### Historical Roman Territorial Boundaries

Historical territorial reconstructions were collected from two geographic sources:

- [Roman Empire Cultural Shapefiles](https://www.arcgis.com/) — ArcGIS Feature Service containing historical territorial boundary layers.
- [Roman Empire Map](https://roman-empire.net/) — GeoJSON boundary data used for selected Republican-era reconstructions.

Nine historical snapshots were used, spanning 264 BC through 314 AD.

### Settlement and Infrastructure Data

Settlement locations and associated historical attributes were obtained from the [Pleiades Gazetteer](https://pleiades.stoa.org/).

The data include geographic coordinates, temporal attributes, and specialized feature classifications. These classifications were used to examine the relationships between battles and ports, temples, forts, amphitheaters, and theaters.

---

## Analytical Approach

The project uses several complementary spatial statistical approaches.

- **Complete Spatial Randomness (CSR):** Establishes whether observed battle locations are more spatially clustered than a uniform random distribution.
- **Settlement-Based Modeling:** Uses kernel density estimation (KDE) to construct a settlement-conditioned spatial distribution.
- **Territorial Boundary Analysis:** Evaluates battle proximity to historical Roman territorial perimeters using settlement-conditioned and boundary-weighted simulations.
- **Infrastructure Proximity Analysis:** Compares battle distances to specialized settlement features against settlement-based expectations.
- **Classification-Based Infrastructure Models:** Uses infrastructure-weighted simulations to investigate differences between external and civil conflicts.

Monte Carlo simulations are used throughout the project to compare observed spatial statistics against alternative spatial distributions.

---

## Acknowledgments

This project was completed as a final GIS research project for PPOL 6805 / DSAN 6750 at Georgetown University.

Historical geographic data and research resources were provided by Wikidata, Pleiades, and the geographic boundary datasets referenced above.

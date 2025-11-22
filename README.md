# MEG — ERFs, Sources & TF (Brainstorm Median-nerve)
[![License](https://img.shields.io/github/license/andraderenew/meg_erfs-sources_brainstorm_median-nerve)](LICENSE)
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.XXXXXXX-blue)](#cite-this-work)
[![Pages](https://img.shields.io/website?url=https%3A%2F%2Fandraderenew.github.io%2Fmeg_erfs-sources_brainstorm_median-nerve%2F)](https://andraderenew.github.io/meg_erfs-sources_brainstorm_median-nerve/)
![Release](https://img.shields.io/github/v/release/andraderenew/meg_erfs-sources_brainstorm_median-nerve?include_prereleases)
![Last commit](https://img.shields.io/github/last-commit/andraderenew/meg_erfs-sources_brainstorm_median-nerve)
[![ORCID](https://img.shields.io/badge/ORCID-0000--0001--5627--579X-A6CE39)](https://orcid.org/0000-0001-5627-579X)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Profile-4285F4)](https://scholar.google.es/citations?hl=es&user=Nl3ApFEAAAAJ)

**One-line:** Reproduce Brainstorm’s median-nerve tutorial: ERFs, source imaging (dSPM/sLORETA), and time–frequency.

## Overview
Reproduce **Brainstorm median-nerve**: sensor-level ERFs, source imaging (**dSPM/sLORETA**), and time–frequency at sources.

## Data & subset
See `DATA_SOURCES.md`. Suggested: 1 subject; tiny footprint (minutes of MEG).

## Pipeline
Import anatomy / coreg → forward model (BEM/overlapping spheres) → inverse (dSPM/sLORETA) → ERFs + TF → figures.

## Results (to be filled)
- ERFs at sensor level  
- Source map at peak; TF in sources

## Reproducibility
- Versions: see `env/TOOL_VERSIONS.md`  
- Steps: “Follow Brainstorm pipeline → export report → figures.”  
- Limits: single-subject demo

## Cite this work
See `CITATION.cff` (add DOI after first Release).

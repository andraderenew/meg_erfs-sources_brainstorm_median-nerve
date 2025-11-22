# MEG: ERFs, Sources & TF (Brainstorm Median-nerve)

**Goal:** Reproduce the Brainstorm median-nerve tutorial: ERFs, source imaging (dSPM/sLORETA), and time–frequency at sources.

---

## Snapshot
- **Dataset:** Brainstorm “Median-nerve” (didactic, one subject)
- **Local subset:** 1 subject · **Disk:** small (minutes of MEG)
- **Tools:** Brainstorm (+ FreeSurfer anatomy if available)
- **Status:** <planned / in progress / complete>
- **Last updated:** <YYYY-MM-DD>

---

## Data
- **Source:** Brainstorm tutorial data (public).  
- **What I downloaded:** the minimal package.  
- **Layout:** Brainstorm protocol folder.

---

## Pipeline (high-level)
1) Import anatomy / coreg MEG-MRI  
2) Forward model (BEM/overlapping spheres)  
3) Inverse (dSPM/sLORETA), ERFs  
4) TF in sources; optional connectivity

---

## Results (to be filled)
- Figure: ERFs at sensor level  
- Figure: source map at peak; TF plot

---

## Reproducibility
- Versions in `env/TOOL_VERSIONS.md`.  
- Steps: “Follow Brainstorm pipeline → export report → figures.”  
- Limitations: single-subject demo.

---

**Author:** Rene Andrade Rey · 🧪 ORCID: https://orcid.org/0000-0001-5627-579X · 🌐 Scholar: https://scholar.google.es/citations?hl=es&user=Nl3ApFEAAAAJ

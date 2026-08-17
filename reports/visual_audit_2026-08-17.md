# Visual audit — Brainstorm median-nerve MEG results

Audit date: 2026-08-17

## Scope

This audit reviews the three public PNG result figures currently tracked in the repository.

The audit is visual and provenance-oriented. It is not an independent numerical replication because the repository does not archive the Brainstorm database, numerical source files, time-frequency matrices, processing scripts, or the exact Brainstorm build used for the original analysis.

## Figure 1 — sensor-space field at 20 ms

File:

`results/figures/fig1.png`

SHA256:

`f44fa49457f94436a9859aa8a2598e4a9e55fe9c46224066ef1387ec26209a8d`

Image size:

710 × 556 pixels.

### Visual findings

- The figure explicitly displays a time point of 20 ms.
- A structured positive/negative sensor-space field pattern is visible.
- The pattern is spatially organized rather than diffuse or obviously artifactual.
- The screenshot therefore supports the claim that an early sensor-space response was inspected around 20 ms.

### Interpretation boundary

The image alone does not contain enough metadata to independently identify the response as the N20m component.

The defensible description is therefore:

> Early somatosensory sensor-field pattern at approximately 20 ms.

Its latency is compatible with the expected N20m time range, but formal component identification is not independently validated by this repository.

## Figure 2 — cortical source map at 20 ms

File:

`results/figures/fig2_sources_20ms.png`

SHA256:

`33d6459fb2349b802bc541b93406eda4150a96d6cad17d25c6ed77a1d8420584`

Image size:

1850 × 1016 pixels.

### Visual findings

- The figure explicitly displays 20 ms.
- A spatially localized cortical source pattern is visible.
- The displayed scale is positive and unitless.
- The screenshot is consistent with a normalized source estimate.

### Interpretation boundary

The PNG itself does not encode the inverse-solution method.

The identification of the result as dSPM therefore comes from the recorded Brainstorm workflow settings, not from independent information embedded in the exported image.

No source coordinates, regional values, peak table, source matrix, or statistical threshold table are archived.

## Figure 3 — sensor-level time-frequency power

File:

`results/figures/fig3_timefrequency_sensor_MEG1133.png`

SHA256:

`703eb22f9a1f4e27c193fda600f8edf5bd5a0159c26571bb7d086407334145dc`

Image size:

623 × 563 pixels.

### Visual findings

- The figure title identifies MEG sensor 1133.
- The figure title identifies a 4–80 Hz power analysis.
- The displayed time range is approximately -100 to 300 ms.
- A vertical marker is visible at stimulation onset (0).
- Power is strongest at low frequencies in the exported view.

### Interpretation boundary

The screenshot does not independently identify the time-frequency transform as Morlet.

The Morlet method comes from the recorded Brainstorm processing settings.

The exported image does not display baseline-normalized units. The public documentation therefore describes this figure as raw power and does not interpret it as event-related percentage or decibel change.

## Overall audit conclusion

**VISUAL AUDIT: PASS WITH DOCUMENTED LIMITATIONS**

The three public figures are internally consistent with the documented Brainstorm median-nerve workflow and provide qualitative evidence for:

1. an early sensor-space response around 20 ms;
2. a cortical source estimate at approximately the same latency; and
3. sensor-level 4–80 Hz power at MEG 1133.

The repository does not support independent numerical reproduction of these results.

Reproducibility should therefore be described as procedural/documentary rather than exact numerical reproducibility.

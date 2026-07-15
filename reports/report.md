# Mini-Report — MEG Median-Nerve (Brainstorm)

## Aim
Reproduce a compact Brainstorm median-nerve MEG workflow and document results across three complementary analysis levels: sensor-space topography, source reconstruction, and time–frequency power.

## Data
- Dataset: Brainstorm **Median-nerve** tutorial dataset.
- Subset: **1 subject**.
- Condition reported here: **Left median-nerve** trials.
- Epoch window: **-100 to 300 ms** relative to stimulation onset.
- Raw MEG and anatomy are not committed to this repository.

## Methods
Tools: **MATLAB** and **Brainstorm**.

Pipeline:
1. Import the tutorial dataset into a Brainstorm protocol.
2. Epoch Left median-nerve events from **-100 to 300 ms** and compute the trial average (ERF).
3. Inspect the early sensor-level response around **20 ms**.
4. Estimate noise covariance from the **-100 to 0 ms** baseline interval.
5. Compute a minimum-norm inverse solution with **dSPM**.
6. Compute **Morlet time–frequency power from 4 to 80 Hz** at representative sensor **MEG 1133**.
7. Export lightweight PNG figures for the portfolio.

## Results
- **Fig 1:** Sensor-level topography around **20 ms**, saved as `results/figures/fig1.png`.
- **Fig 2:** **dSPM** source distribution around **20 ms**, saved as `results/figures/fig2_sources_20ms.png`.
- **Fig 3:** **Morlet time–frequency power (4–80 Hz)** at sensor **MEG 1133**, over **-100 to 300 ms**, saved as `results/figures/fig3_timefrequency_sensor_MEG1133.png`.
- The time–frequency figure displays **raw power**; no baseline normalization was applied in the exported view.

## QC
- Stimulation onset was checked at **t = 0 ms**.
- The early sensor-level response and topographic pattern were visually inspected around **20 ms**.
- The dSPM source result was inspected at approximately the same early-response time point.
- The Morlet result was checked across the full **4–80 Hz** and **-100 to 300 ms** display range.

## Limitations
- Single-subject tutorial dataset; no group-level inference is performed.
- Source localization accuracy depends on the tutorial anatomy/head-model assumptions.
- The time–frequency figure shows raw power and therefore retains the expected frequency-dependent spectral profile; it should not be interpreted as baseline-normalized event-related power change.

## Reproducibility
- Software and environment information: `env/TOOL_VERSIONS.md`.
- High-level rerun steps: `README.md`.
- Data provenance and policy: `DATA_SOURCES.md`.

# Protein Stability Curves

An interactive teaching tool for protein thermodynamics. Students work through a six-step guided lesson on the protein stability curve (ΔG of unfolding versus temperature), predicting each answer before revealing it, while a live model responds.

**Live page:** https://kuhfeldrf.github.io/protein_stability_curve/

## What it covers

1. Reading the stability curve: Tm and the sign of ΔG
2. From ΔG to molecules: K = [U]/[N] = exp(−ΔG/RT) and the fraction folded
3. Where ΔG comes from: ΔHref, TΔSref, ΔCp(T − Tref) and TΔCp·ln(T/Tref), the yellow columns of the class spreadsheet
4. Why maximum stability (Ts) is not at Tm
5. How ΔCp bends the curve and causes cold denaturation (Tc)
6. A destabilizing mutation (ΔΔG)

It also maps the ideas onto the ligand-binding lecture (K, fractional saturation, Kd as the half-point, all-or-none binding versus two-state unfolding).

## Model

Two-state unfolding N ⇌ U with temperature-independent ΔCp:

ΔG(T) = ΔHm(1 − T/Tm) + ΔCp[(T − Tm) − T·ln(T/Tm)]

Default inputs match the class spreadsheet: Tm = 88.5 °C, ΔHm = 435 kJ/mol, ΔCp = 7.32 kJ/(mol·K). The page converts °C to K with 273.15; the spreadsheet uses 273, which changes ΔG by less than 0.02 kJ/mol between 0 and 100 °C.

## Running it

`index.html` is a single self-contained file. Open it in a browser, or serve the repository with GitHub Pages.

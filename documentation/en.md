<!-- ELUCENIA technical documentation · escore-air-apendicite · en · no clinical/professional/rights approval -->

# AIR score (Appendicitis Inflammatory Response)

[conditions, sources and permissions](https://elucenia.org/en/tools/escore-air-apendicite)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Vomiting

`vomito`

### Right iliac fossa pain

`dor`

### Rebound tenderness or muscular guarding

`defesa`

- `0` — Absent
- `1` — Mild
- `2` — Moderate
- `3` — Intense

### Temperature ≥ 38.5 °C

`temp`

### Neutrophils

`neut`

- `0` — \< 70%
- `1` — 70 to 84%
- `2` — ≥ 85%

### White blood cells

`leuco`

- `0` — \< 10,000/mm³
- `1` — 10,000 to 14,900/mm³
- `2` — ≥ 15,000/mm³

### C-reactive protein

`pcr`

- `0` — \< 10 mg/L
- `1` — 10 to 49 mg/L
- `2` — ≥ 50 mg/L

## Method edition

AIR by Andersson (2008), with Tables 2 and 7 corrected by the 2012 erratum: seven components, total 0–12, CRP in mg/L; original groups 0–4, 5–8 and 9–12. The lower-cutoff change proposed in 2021 has not been applied.

## Documented formula

Vomiting (1) + right iliac fossa pain (1) + mild (1), moderate (2) or severe (3) peritoneal irritation + temperature ≥38.5 °C (1) + neutrophils 70–84% (1) or ≥85% (2) + leukocytes 10,000–14,900 (1) or ≥15,000 (2) + CRP 10–49 (1) or ≥50 mg/L (2). Total 0 to 12.

## Limits and population

The 2008 AIR was studied in people admitted with suspected appendicitis; part of the cohort remained in the indeterminate group and required further investigation. Only the abstract of the original 2008 article was read. The 2012 erratum was read directly: its Tables 2 and 7 correct CRP concentrations and document the points, units and original groups. The numerical check is limited to summing the seven already selected components; it does not approve clinical groups or diagnostic, imaging or surgical decisions. The 2021 revision proposed low risk at a score \<4, distinct from the original 0–4 group; that change has not been applied in this edition. Minimum age, exclusions and the complete protocol were not confirmed by reading the 2008 abstract. Unobserved findings must not be treated as absent. Independent professional clinical and language review and authorization of instrument rights have not been performed.

## References

- [Andersson M, Andersson RE. The appendicitis inflammatory response score: a tool for the diagnosis of acute appendicitis that outperforms the Alvarado score. World J Surg, 2008.](https://doi.org/10.1007/s00268-008-9649-y)

- [Di Saverio S et al. Diagnosis and treatment of acute appendicitis: 2020 update of the WSES Jerusalem guidelines. World J Emerg Surg, 2020.](https://doi.org/10.1186/s13017-020-00306-3)

- [Andersson M, Andersson RE. Erratum to: The Appendicitis Inflammatory Response Score: A Tool for the Diagnosis of Acute Appendicitis that Outperforms the Alvarado Score. World J Surg, 2012;36:2269–2270. Corrected Tables 2 and 7.](https://doi.org/10.1007/s00268-012-1679-9)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Low probability (0 to 4)

High with reassessment if symptoms persist, in a patient with assured follow-up.


### 2

Indeterminate probability (5 to 8)

Active observation with clinical and laboratory reassessment and/or imaging examination.


### 3

High probability (9 to 12)

Surgical evaluation.


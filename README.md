#  DENV-2 Mutation Checking with Vaccine References

##  Overview

This project investigates the **genetic variation of Bangladesh DENV-2 sequences** in comparison with selected DENV-2 vaccine/reference sequences.

The analysis focuses on sequence-level **mutation, indel, and identity comparison** using complete DENV-2 genome sequences.

---

##  Objectives

* Identify and filter **DENV-2 sequences** from the dengue dataset.
* Select available **complete DENV-2 genomes** from Bangladesh.
* Compare Bangladesh DENV-2 sequences with selected vaccine/reference sequences.
* Measure **sequence identity, substitutions, and indels** through sequence alignment.

---

## Data & References

### Bangladesh Dengue Dataset

* **664 dengue virus sequences**
* Multiple serotypes: DENV-1, DENV-2, DENV-3, and DENV-4
* **278 DENV-2 sequences**
* **22 complete DENV-2 genomes** used for genome-level comparison

### DENV-2 References

| Reference             | Accession    | Type                             |
| --------------------- | ------------ | -------------------------------- |
| TAK-003 / PDK-53      | `KU725664.1` | Complete genome                  |
| CYD-TDV DENV-2        | `KX239895.1` | Partial surface-protein sequence |
| TV 003 / New Guinea C | `KM204118.1` | Complete genome                  |

---

## Methodology

```text
Dengue Dataset
      ↓
Data Cleaning & Standardization
      ↓
Serotype Identification
      ↓
DENV-2 Filtering
      ↓
Complete Genome Selection
      ↓
Reference/Vaccine Sequence Collection
      ↓
Sequence Alignment
      ↓
Mutation + Indel + Identity Analysis
```

The analysis was performed using **Python, Pandas, Biopython, and Pairwise Sequence Alignment**.

* **Global alignment** was used for complete genome comparisons.
* **Local alignment** was used for the partial CYD-TDV reference sequence.

---

## Key Findings

For the comparison with **TAK-003 / PDK-53 (KU725664.1)**:

* Mean substitutions: **~1158.77**
* Mean sequence identity: **~88.99%**
* Identity range: **78.15% – 99.48%**

For the selected Bangladesh DENV-2 sequence `OZ484492.1`:

| Reference        | Sequence Identity |
| ---------------- | ----------------: |
| TAK-003 / PDK-53 |           ~89.96% |
| CYD-TDV DENV-2   |            92.39% |
| TV 003           |           ~88.80% |

These results indicate **measurable genetic variation** between the analyzed Bangladesh DENV-2 sequences and the selected reference sequences.

---

## Important Note

Sequence identity and nucleotide mutations **alone cannot determine vaccine effectiveness or vaccine failure**.

Therefore, the current analysis should be considered a **preliminary genetic comparison**, rather than direct evidence of vaccine mismatch.

Further analysis such as **amino-acid mutations, E-protein analysis, epitope comparison, phylogenetic analysis, and antigenic/neutralization data integration** would provide stronger biological interpretation.

---



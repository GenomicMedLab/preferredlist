# CIViC Analysis Notes

The CIViC resource is the preferred resource for the 
[ClinGen Somatic Cancer Pediatric Taskforce](https://clinicalgenome.org/working-groups/somatic/pediatric-task-team/).
They have been working to create pediatric-disease-specific entries in the CIViC data model, and this serves as an
easily updatable resource we may utilize to advance our own efforts.

## Evidence selection criteria
CIViC evidence [was searched](https://civicdb.org/search/evidence/7aa158ab-1aa4-4d48-a5a0-3a07f9d5580f) under the following criteria:
- Disease name contains "Pediatric"
  - Not all pediatric terms are linked to ontological concepts yet
- Evidence is level B (Clinical trials) or level A (Validated association)
- Evidence is accepted (has been reviewed and approved by a non-authoring editor)
- Evidence is trust rating >= 3 stars
- Evidence direction supports

## Evidence to passlist roll-up
The [resulting list of variants](../../data/CIViC_evidence_2020-09-18T16_09_39.csv) was small, mostly categorical.
- Fusions:
  - KIAA1549-BRAF (Pediatric Low-grade Glioma (PLGG))
- Amplifications:
  - MYB (PLGG)
- Deletions:
  - ATRX (PLGG)
  - CDKN2A (PLGG)
  - IKZF1 (Pediatric B-cell Acute Lymphoblastic Leukemia (PB-ALL))
- Mutations:
  - H3-3A (PLGG)
  - IKZF1 (PB-ALL)
- Hotspots:
  - BRAF V600E (PLGG)
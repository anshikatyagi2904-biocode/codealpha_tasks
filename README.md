# CodeAlpha Bioinformatics Internship Tasks

This repository contains all bioinformatics tasks completed as part of the
CodeAlpha internship program.

---

## Task 1 — DNA / Protein Sequence Analysis

**File:** `Task1_Analysis_Report.docx`

### Protein Studied
| Field | Detail |
|---|---|
| Protein | Cytochrome c |
| Gene | CYCS |
| Organism | *Homo sapiens* |
| UniProt Accession | P99999 |
| Sequence Length | 105 amino acids |

### What Was Done
- Retrieved the canonical human Cytochrome c sequence from UniProt (P99999)
- Performed BLASTp search against the NCBI non-redundant (nr) protein database
- Analyzed top 4 orthologous hits across diverse taxa:
  - *Pan troglodytes* (Chimpanzee) — 99% identity
  - *Mus musculus* (Mouse) — 91% identity
  - *Gallus gallus* (Chicken) — 84% identity
  - *Saccharomyces cerevisiae* (Yeast) — 72% identity
- Interpreted conserved residues (Cys14, Cys17, His18, Met80, Phe82) in
  terms of heme binding and electron transfer function
- Discussed evolutionary conservation, purifying selection, and molecular
  clock properties of Cytochrome c

### Key Findings
- Sequence identity decreases predictably with phylogenetic distance,
  validating Cytochrome c as a molecular clock protein
- All BLAST hits returned E-values between 10⁻⁴⁵ and 10⁻⁷³, confirming
  true evolutionary homology
- Functionally critical residues are 100% conserved even across 1.5 billion
  years of eukaryotic evolution

### Tools Used
- [UniProt](https://www.uniprot.org/) — sequence retrieval
- [NCBI BLASTp](https://blast.ncbi.nlm.nih.gov/) — homology search



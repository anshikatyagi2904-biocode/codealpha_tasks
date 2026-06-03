# CodeAlpha Bioinformatics Internship Tasks

**Intern:** Anshika Tyagi
**Program:** CodeAlpha – 1 Month Bioinformatics Internship
**Repository:** All completed task reports with analysis, results, and visualizations.

---

## Tasks Overview

| Task | Title | Protein | Tool(s) | File |
|------|-------|---------|---------|------|
| Task 1 | DNA / Protein Sequence Analysis | Cytochrome c (*Homo sapiens*, P99999) | NCBI BLASTp | `Task 1.docx` |
| Task 2 | Multiple Sequence Alignment | Hemoglobin β-subunit (5 mammalian species) | Clustal Omega | `Task 2.docx` |
| Task 3 | Protein Structure Prediction & Visualization | Myoglobin (*Homo sapiens*, P02144) | UCSF Chimera, PDB 3RGK | `Task 3.docx` |

---

## Task 1 — DNA / Protein Sequence Analysis

**File:** `Task 1.docx`

### Protein Studied

| Field | Detail |
|-------|--------|
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
- Interpreted conserved residues (Cys14, Cys17, His18, Met80, Phe82) in terms of heme binding and electron transfer function
- Discussed evolutionary conservation, purifying selection, and molecular clock properties of Cytochrome c

### Key Results

| Hit | Species | Identity | E-value |
|-----|---------|----------|---------|
| 1 | Chimpanzee | 99% | 2e-73 |
| 2 | Mouse | 91% | 3e-67 |
| 3 | Chicken | 84% | 8e-59 |
| 4 | Yeast | 72% | 2e-45 |

> Cytochrome c shows >72% identity even after ~1.5 billion years of eukaryotic divergence — one of the highest conservation rates known for any protein.

---

## Task 2 — Multiple Sequence Alignment

**File:** `Task 2.docx`

### Protein Family Studied

Hemoglobin Beta Subunit (β-Globin) — 5 mammalian species, all 147 amino acids.

| UniProt ID | Organism | Gene |
|------------|----------|------|
| P68871 | *Homo sapiens* (Human) | HBB |
| P02088 | *Mus musculus* (Mouse) | Hbb-b1 |
| P02091 | *Rattus norvegicus* (Rat) | Hbb |
| P02070 | *Bos taurus* (Bovine) | HBB |
| P02062 | *Equus caballus* (Horse) | HBB |

### What Was Done
- Retrieved 5 canonical β-globin FASTA sequences from UniProtKB/Swiss-Prot
- Performed Multiple Sequence Alignment using Clustal Omega (BLOSUM62, gap open 10.0)
- Analyzed conservation statistics and identified fully conserved functional motifs
- Constructed pairwise identity matrix across all 5 species

### Key Results

| Metric | Value |
|--------|-------|
| Fully conserved residues (*) | ~89 (≈59%) |
| Strongly similar (:) | ~28 (≈19%) |
| Average pairwise identity | ~83–87% |
| Highest pairwise identity | Mouse vs. Rat — 91.2% |
| Lowest pairwise identity | Rat vs. Bovine — 79.6% |

**Conserved functional motifs identified:** proximal His F8 (His92), distal His E7 (His63), LLVVYPWTQR core motif, C-terminal His146 (Bohr effect).

---

## Task 3 — Protein Structure Prediction & Visualization

**File:** `Task 3.docx`

### Protein Studied

| Field | Detail |
|-------|--------|
| Protein | Myoglobin |
| Gene | MB |
| Organism | *Homo sapiens* |
| UniProt Accession | P02144 |
| PDB Entry | 3RGK (X-ray, 1.65 Å) |
| Sequence Length | 154 amino acids |

### What Was Done
- Retrieved the crystal structure of human Myoglobin from PDB (entry 3RGK, 1.65 Å resolution)
- Loaded and visualized the structure in **UCSF Chimera**
- Generated ribbon and heme-binding site views of the globin fold
- Identified and annotated the 8 alpha-helices (A–H) and key functional residues

### Secondary Structure Summary

| Helix | Residues | Function |
|-------|----------|----------|
| A | 4–18 | N-terminal helix; heme environment |
| B | 20–35 | Packs against heme propionate groups |
| E | 58–77 | Contains His64 (distal His); O₂ binding |
| F | 86–96 | Contains His93 (proximal His); heme Fe coordination |
| H | 124–148 | Longest helix; C-terminal |

**Key residues:** His93 (proximal ligand), His64 (distal ligand), Val68 (steric gating), Phe43 (heme insertion).

---

## Tools & Databases Used

| Tool / Database | Purpose |
|-----------------|---------|
| [UniProtKB](https://www.uniprot.org) | Protein sequence retrieval |
| [NCBI BLASTp](https://blast.ncbi.nlm.nih.gov) | Sequence homology search |
| [Clustal Omega](https://www.ebi.ac.uk/Tools/msa/clustalo/) | Multiple sequence alignment |
| [RCSB PDB](https://www.rcsb.org) | 3D structure retrieval |
| [UCSF Chimera](https://www.cgl.ucsf.edu/chimera/) | Molecular visualization |

---

## Repository Structure

```
codealpha_tasks/
├── README.md
├── Task 1.docx       # Cytochrome c – BLASTp sequence analysis
├── Task 2.docx       # Hemoglobin β-subunit – Multiple sequence alignment
└── Task 3.docx       # Myoglobin – Structure visualization (UCSF Chimera)
```


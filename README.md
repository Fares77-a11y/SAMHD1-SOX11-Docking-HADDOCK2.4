# SAMHD1-SOX11-Docking-HADDOCK2.4
Protein–protein docking of SAMHD1 and SOX11 using HADDOCK 2.4: comparative analysis of random vs. centroid-based ligand placement, cluster scoring, and PyMOL/PDBsum interaction mapping.

# 🔬 SAMHD1–SOX11 Docking Analysis (HADDOCK 2.4)

This project compares two protein–protein docking strategies (random vs. centroid-restrained) for the SAMHD1–SOX11 complex using the HADDOCK 2.4 platform. Structural insights were supported by interface analysis via PDBsum and PyMOL visualization.

---

## 🧪 Overview

- **Proteins**: SAMHD1 and SOX11 (renumbered chains, preprocessed via PyMOL and PDB-tools)
- **Docking Tool**: HADDOCK 2.4 (https://wenmr.science.uu.nl/haddock2.4/)
- **Protocols**:
  - Random ligand placement
  - Centroid-restrained placement (interface-based)
- **Analysis**:
  - Cluster scoring
  - PDBsum-based interaction breakdown (H-bonds, salt bridges, hydrophobic patches)
  - Visualized with cartoon overlays and interface plots

---

## 📊 Results Summary

| Cluster        | HADDOCK Score | Buried Surface Area (Å²) | Electrostatic Energy | VdW Energy | Z-Score |
|----------------|----------------|----------------------------|----------------------|------------|---------|
| Random (200)   | -110.2         | 1622.4                     | -124.7               | -44.3      | -1.9    |
| Center (361)   | -98.4          | 1450.1                     | -110.3               | -41.8      | -1.3    |

---

## 🧬 Structural Visualizations

| Molecule | View |
|----------|------|
| SAMHD1 (Unbound) | ![](figures/unbound_SAMHD1.png) |
| SOX11 (Unbound)  | ![](figures/unbound_SOX11.png) |
| Docked Complex (Random) | ![](figures/cluster200_docked.png) |
| Docked Complex (Centroid) | ![](figures/cluster361_docked.png) |

---

## 📊 Cluster Score Tables

- [random_haddock_clusters.tsv](results/random_haddock_clusters.tsv)
- [centered_haddock_clusters.tsv](results/centered_haddock_clusters.tsv)

Each file contains:
- Cluster ID
- HADDOCK score
- Z-score
- Buried surface area (BSA, Å²)

---

## ⚙️ HADDOCK Terminal Setup

Local `run.param` files are available under `src/` for both docking protocols:
- `run_random.param`
- `run_center.param`

---

## 👨‍💻 Author

**Fares Ibrahim**  
Structural Bioinformatics | Protein–Protein Docking | Cancer Systems Biology

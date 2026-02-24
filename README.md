# Portfolio Académique - Marwane TCHABANNA KOUDJOWOU
Modeling Red Blood Cell Dynamics using PINNs 🩸💻
This repository contains my Master 1 research project in Numerical Modeling and Analysis at the University of Montpellier. The core objective is to leverage Physics-Informed Neural Networks (PINNs) to infer the mechanical properties of Red Blood Cells (RBCs) based on their dynamics under flow conditions.
---
## 👨‍🏫 Supervision
Advised by:

-Vanessa Lleras (Associate Professor, University of Montpellier / IMAG)

-Simon Mendez (CNRS Research Scientist / IES)
## 🔬 Scientific Context
Red blood cell deformability is a critical biomarker of health. Pathologies such as sickle cell anemia or malaria modify the mechanical properties of the cell membrane, making them less capable of circulating through microvessels. This project aims to develop a non-invasive diagnostic tool by using AI to solve inverse problems in biophysics
## 🎯 Step 1: The Keller and Skalak (KS) Model
The first milestone of this project is to implement and solve the foundational Keller and Skalak (1982) model
Model Overview
The KS model describes the motion of a fluid ellipsoid with a fixed shape in a simple shear flow. It successfully reproduces two essential motion regimes:
  1-Tumbling: The cell rotates as a rigid body
  2-Tank-treading: The membrane rotates around the internal cytoplasm while the cell maintains a stable orientation
Numerical Objectives

 -PINNs Implementation: Translate the system of coupled Ordinary Differential Equations (ODEs) from the KS model into the loss function of a neural network.
 
 -Parameter Inference: Train the network to recover physical parameters (such as viscosity ratios or shear rates) from angular trajectory data.
 
 -Validation: Benchmark the PINN results against the analytical solutions provided in Section 6 of the original Keller (1982) paper.
##  🛠️ Tech Stack
- Python 🐍

DeepXDE / PyTorch (for PINN implementation)

NumPy / Matplotlib (for numerical analysis and visualization)

## 📚 Key References
Keller, S. R., & Skalak, R. (1982). Motion of a 2D fluid ellipsoid in a 2D shear flow.

Abkarian, M., & Viallat, A. (2016). On The Importance Of Red Blood Cells Deformability In Blood Flow. Chapter 1.


---

tchabanna-academic-portfolio/
├── README.md               <-- Présentation générale (ce qu'on a rédigé)
├── LICENSE                 <-- Licence (ex: MIT) pour protéger votre code
├── docs/                   <-- Bibliographie et notes théoriques
│   ├── notes_keller_skalak.md
│   └── resume_abkarian_2016.md
├── src/                    <-- Scripts Python (le cœur du projet)
│   ├── keller_skalak_analytical.py  <-- Solutions de référence
│   └── rbc_pinn_solver.py           <-- Votre modèle PINN
├── data/                   <-- Données synthétiques ou expérimentales
├── notebook/               <-- Expérimentations interactives (Jupyter)
│   └── validation_pinn_vs_analytical.ipynb
└── assets/                 <-- Images, schémas et animations
    └── rbc_motion.gif
## 🚀 Organisation du Projet

* **[docs/](./docs)** : Synthèses théoriques des modèles de Keller-Skalak (1982) et Abkarian (2016).
* **[src/](./src)** : Implémentation des Physics-Informed Neural Networks (PINNs) pour la résolution des systèmes d'EDO.
* **[notebook/](./notebook)** : Comparaisons graphiques entre les prédictions numériques et les solutions analytiques exactes.
---

## 🚀 Project Structure

docs/: Theoretical syntheses and technical notes on the Keller-Skalak (1982) and Abkarian (2016) models. This section details the derivation of the coupled ODEs and the physical meaning of the parameters.
src/: Core source code including the implementation of Physics-Informed Neural Networks (PINNs) to solve the system of Ordinary Differential Equations (ODEs).
notebook/: Interactive Jupyter notebooks for data visualization and benchmarking. These contain quantitative comparisons between the PINN predictions and the exact analytical solutions provided in the literature

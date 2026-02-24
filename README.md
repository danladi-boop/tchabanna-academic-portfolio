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

## Organisation du Portfolio

- **`index.html`** : Page d'accueil du portfolio, présentant une vue d'ensemble de mes travaux.
- **`style.css`** : Feuille de style pour le design du site.
- **`/travaux/`** : Dossier contenant mes projets académiques, organisés par thème :
  - Optimisation
  - Analyse Numérique
  - Analyse Fonctionnelle
  - Équations aux Dérivées Partielles (EDP)
  - Géométrie Différentielle
- **`/pdf/`** : Dossier contenant les versions PDF de mes travaux pour un accès facile et une lecture hors ligne.

---

## Comment Utiliser ce Portfolio ?

- **Navigue** à travers les projets pour découvrir mes travaux.
- **Télécharge** les PDFs pour une lecture détaillée.
- **Contacte-moi** pour toute question, suggestion ou opportunité de collaboration.

---

## Philosophie

> *"J'ai une dette envers la nature et la communauté académique. Je souhaite la payer en partageant mes connaissances, en écoutant et en apprenant des autres pour œuvrer ensemble au bien-être et à l'avancement de la science."*

---

## Contact

Pour toute question, suggestion ou collaboration, n'hésitez pas à me contacter :
- Email : marwane.tchabanna@etu.umontpellier.fr
- GitHub : [danladi-boop](https://github.com/danladi-boop)
- Site : https://danladi-boop.github.io/tchabanna-academic-portfolio/
---

Merci de visiter mon portfolio, et j'espère que ces travaux pourront t'être utiles !

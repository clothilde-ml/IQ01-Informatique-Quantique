# Quantum Computing — Between Technological Revolution and Self‑Fulfilling Prophecy

## Solving the Travelling Salesman Problem

*This repository was created as part of a group project at UTC (Université de Technologie de Compiègne). The report, slides, and notebooks are written in French. The notebooks were designed to be accessible to anyone with a background in linear algebra.*

---

## 🇫🇷 Présentation

Ce dépôt rassemble le travail d'un projet de groupe portant sur l'application des **algorithmes quantiques** au problème du voyageur de commerce (TSP), abordé sous ses deux formes :

- **Version NP-Complet** : résolution par l'**algorithme de Grover**, avec explications visuelles détaillées du fonctionnement
- **Version NP-Difficile** : reformulation via **QUBO** et résolution par **QAOA**

Le rapport s'ouvre sur une introduction historique à l'informatique quantique : ses balbutiements, sa naissance, et son développement jusqu'à sa massification.

---

## Contenu du dépôt

```
Rapport.pdf                                  — rapport complet du projet de groupe
Slides-Presentation.pdf                      — diapositives de la présentation orale
notebooks/                                   — notebooks personnels
    ├── 1-Framewoks-Quantique.ipynb          — tour d'horizon des frameworks quantiques
    ├── 2-Fondamentaux-Quantique.ipynb       — fondements de la programmation quantique
    ├── 3-Grover.ipynb                       — implémentation détaillée de l'algorithme de Grover
    └── generate-distance-matrix.ipynb       — annexe : matrice de distance (théorique) en quantique
```

---

## A propos des notebooks du répertoire

Les notebooks de ce répertoire ne constituent que ma partie du travail dans le projet de groupe. Ils couvrent brièvement les principaux frameworks quantiques disponibles en Python (**Qiskit, Cirq, PennyLane, D-Wave** et **QuTiP**) avant de se concentrer sur les fondamentaux et l'implémentation de Grover.

Ils sont accessibles à toute personne ayant des bases en algèbre linéaire. Les concepts sous-jacents aux qubits et aux opérations quantiques y sont introduits et expliqués, de sorte qu'aucun prérequis en physique quantique n'est nécessaire.

Pour plus de détail sur les implémentations par QUBO et par QAOA, je vous invite vivement à vous intéresser au travail de mes collaboratrices disponible sur leur GitHub :

- [Page MAGNIER--SLIMANI](https://github.com/Page-MS)
- [Lauranne FOSSAT](https://github.com/lau-fst)

---

## Note sur les limites de l'implémentation

Le notebook `generate-distance-matrix.ipynb` donné en annexe permet de montrer les limites de l'algorithme de Grover dans le cas du problème du TSP, en ce qui concerne le nombre de qubits parallèles nécessaires pour implémenter la matrice de distance.

Si vous avez connaissance d'une approche permettant de contourner cette contrainte de façon réalisable, je serais sincèrement curieuse d'en discuter. N'hésitez pas à ouvrir une issue ou à me contacter directement.

---

## Dépendances et environnement

Les notebooks sont écrits en **Python** et fournis au format `.ipynb`. 

Leur exécution nécessite l’installation des bibliothèques :

- **Qiskit** (programmation quantique)
- **Qiskit Aer** (simulateur quantique)
- **NumPy** et **Matplotlib**
- **NetworkX** (pour l'affichage d'un graphe - *optionnel*)

Installation recommandée :

```bash
pip install qiskit qiskit-aer numpy matplotlib networkx
```

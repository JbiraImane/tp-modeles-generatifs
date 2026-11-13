# TP Modèles génératifs

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![PyTorch](https://img.shields.io/badge/PyTorch-ee4c2c)

Implémentation, à partir de zéro, des briques de base des modèles génératifs : estimation de distributions, modèles latents linéaires et modèles autorégressifs.

## Sommaire

- [Objectifs](#objectifs)
- [Contenu](#contenu)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Technologies](#technologies)
- [Auteur](#auteur)

## Objectifs

- Estimer des distributions par maximum de vraisemblance (descente de gradient, EM)
- Générer de nouvelles données à partir d'un modèle appris
- Comparer des approches : modèles gaussiens, mélanges, modèles autorégressifs

## Contenu

| Partie | Thème | Méthodes |
|---|---|---|
| 1 | Estimation de distributions | Bernoulli, gaussiennes uni/multivariées (Σ = LLᵀ), GMM et algorithme EM |
| 2 | Modèle gaussien pour images | Covariance empirique, ACP, eigen-images, générateur affine G(z) = μ + Az |
| 3 | Modèles autorégressifs | Chaînes de Markov (bigrammes, trigrammes), modèle d'ordre n, lissage de Laplace |

## Installation

```bash
git clone https://github.com/JbiralImane/tp-modeles-generatifs.git
cd tp-modeles-generatifs

python -m venv venv
source venv/bin/activate        # Windows : venv\Scripts\activate

pip install numpy torch scipy scikit-learn matplotlib jupyter
```

## Utilisation

```bash
jupyter notebook tp-modeles-generatifs.ipynb
```

Exécuter les cellules dans l'ordre. Les données MNIST sont téléchargées automatiquement ; en l'absence de connexion, le notebook utilise le jeu de chiffres 8x8 de scikit-learn.

## Technologies

NumPy · PyTorch · SciPy · scikit-learn · Matplotlib

## Auteur

**JbiralImane** : [github.com/JbiralImane](https://github.com/JbiralImane)

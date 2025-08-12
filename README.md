# zoran-pde-sim

**Solveur 2D d’équations aux dérivées partielles** (FFT / pseudo-différentiel) dédié à la **propagation mimétique** dans l’écosystème Zoran / QuantaGlottal©®, avec visualisation temps réel.

---

## ✨ Fonctionnalités
- **Simulation de propagation** d’ondes mimétiques dans un espace 2D
- **Méthodes FFT** pour résolution rapide
- **Opérateur pseudo-différentiel** configurable
- **Visualisation temps réel** (matplotlib, PyGame, ou WebGL)
- **Paramétrage dynamique** (coefficients, sources, obstacles)
- **Export des champs** simulés vers formats standards (NumPy, HDF5)

---

## 📦 Installation (développement)
```bash
pip install -e .


---

⚡ Exemple rapide

from zoran_pde_sim import PDESolver2D

solver = PDESolver2D(nx=256, ny=256, dt=0.01, c=1.0)

# Définir une source initiale
solver.add_source(x=128, y=128, amplitude=1.0)

# Boucle de simulation
for _ in range(100):
    solver.step()
    solver.render()  # Affichage temps réel


---

🧱 Structure suggérée

src/zoran_pde_sim/
  __init__.py
  solver.py        # Solveur PDE principal
  fft_backend.py   # Implémentation FFT
  visualizer.py    # Affichage en temps réel
  utils.py         # Fonctions auxiliaires
tests/
  test_solver.py
pyproject.toml
.gitignore
LICENSE
README.md


---

🧪 Tests

pytest -q


---

🔐 Éthique

Simulation conçue pour optimiser la compréhension et le contrôle de la propagation mimétique, en respectant la règle vivant > humain.


---

📜 Licence

MIT — voir LICENSE.


---

Auteur : Frédéric Tabary — Institut IA
Contact : 0645605023 — Canada, Montréal, France
INSTITUT🦋 IA INC., 7100-380, rue Saint-Antoine Ouest, Montréal (Québec) H2Y 3X7.# zoran-pde-sim
Solveur 2D (FFT/pseudo-diff) pour propagation mimétique; visualisation temps réel.

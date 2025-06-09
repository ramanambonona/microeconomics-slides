# Microéconomie Avancée - Rappels Mathématiques

Ce dépôt contient les rappels mathématiques essentiels pour le cours de Microéconomie Avancée.

## Contenu des Rappels

### 1. Fonctions à plusieurs variables
- Définition : Application de ℝ₊ⁿ vers ℝ
- Notation : $y = f(x_1, \dots, x_n)$

### 2. Dérivées et Dérivées Partielles
- **Dérivée** (1 variable) :
  $$f'(x) = \lim_{\Delta x \rightarrow 0} \frac{f(x+\Delta x)-f(x)}{\Delta x}$$
  
- **Dérivées partielles** (n variables) :
  $$\frac{\partial f}{\partial x_i} = \lim_{\Delta x_i \to 0} \frac{f(\dots, x_i + \Delta x_i, \dots) - f(\dots, x_i, \dots)}{\Delta x_i}$$

### 3. Différentielle Totale
- Variation totale d'une fonction différentiable :
  $$df = \frac{\partial f}{\partial x_1} dx_1 + \cdots + \frac{\partial f}{\partial x_n} dx_n$$

### 4. Concavité et Convexité
- **Fonction concave** :
  $$f(\lambda x + (1 - \lambda)x') \geq \lambda f(x) + (1 - \lambda)f(x')$$
  
- **Fonction convexe** :
  $$f(\lambda x + (1 - \lambda)x') \leq \lambda f(x) + (1 - \lambda)f(x')$$
  
- Critère matriciel (Hessienne) :
  $$H_f(x) = \begin{bmatrix}
  \frac{\partial^2 f}{\partial x_1^2} & \cdots & \frac{\partial^2 f}{\partial x_1 \partial x_n} \\
  \vdots & \ddots & \vdots \\
  \frac{\partial^2 f}{\partial x_n \partial x_1} & \cdots & \frac{\partial^2 f}{\partial x_n^2}
  \end{bmatrix}$$

### 5. Optimisation
- **Conditions d'optimalité** :
  - Premier ordre : $\nabla f(x^*) = 0$
  - Second ordre : 
    - $H_f(x^*)$ définie négative → maximum local
    - $H_f(x^*)$ définie positive → minimum local

- **Optimisation sous contrainte** :
  $$\begin{aligned}
  & \max f(x) \\
  & \text{s.c. } g(x) = c
  \end{aligned}$$
  - Méthode du Lagrangien :
    $$\mathcal{L}(x, \lambda) = f(x) - \lambda (g(x) - c)$$
  - Interprétation de λ : Valeur marginale de la contrainte

### 6. Fonctions Homogènes
- Définition :
  $$f(\lambda x_1, \dots, \lambda x_n) = \lambda^\mu f(x_1, \dots, x_n)$$
- Degré 0 : rendements constants
- Degré 1 : rendements linéaires

## Exemples Clés

### Dérivées partielles
Pour $f(x, y) = x^2 y + 3xy^2$ :
- $\frac{\partial f}{\partial x} = 2xy + 3y^2$
- $\frac{\partial f}{\partial y} = x^2 + 6xy$

### Concavité/Convexité
1. $f(x) = \ln(x)$ : concave ($f''(x) = -1/x^2 < 0$)
2. $f(x) = x^2$ : convexe ($f''(x) = 2 > 0$)

### Optimisation sous contrainte
Problème :
$$\begin{aligned}
& \max xy \\
& \text{s.c. } x + y = 10
\end{aligned}$$

Solution : $(x^*, y^*) = (5, 5)$, $\lambda = 5$

### Homogénéité
1. $f(x, y) = x^2 + y^2$ : degré 2
2. $f(x, y) = x/y$ : degré 0

---

**Enseignant** : Dr. Ramanambonona Ambinintsoa  
**Dernière mise à jour** : 7 juin 2025
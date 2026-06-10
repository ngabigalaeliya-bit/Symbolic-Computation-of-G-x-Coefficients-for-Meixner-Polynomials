# Symbolic Computation of G₂(x) Coefficients for Meixner Polynomials

## Overview

This repository provides Mathematica implementations for the symbolic computation of the coefficients

$$
G_2(x)=A_k x^2+B_k x+D_k,
$$

arising in higher-order Christoffel transformations of Meixner polynomials.

The code computes explicit expressions for the coefficients (A_k), (B_k), and (D_k) for

$$
k=1,2,3,4,5,6,
$$

using determinant representations derived from the corresponding modified orthogonality measures.

The implementation is intended for symbolic investigations related to:

* Meixner orthogonal polynomials;
* Christoffel and Geronimus transformations;
* Kernel and quasi-orthogonal polynomials;
* Interlacing properties of zeros;
* Higher-order spectral transformations.

---

## Mathematical Background

Let

$$
M_n(x;\beta,c)
$$

denote the monic Meixner polynomial with parameters

$$
\beta>0,
\qquad
0<c<1.
$$

The polynomial (G_2(x)) appears in the connection formula relating modified and classical Meixner families. It can be written as

$$
G_2(x)=A_k x^2+B_k x+D_k,
$$

where the coefficients depend on the modification order (k), the parameters (\beta) and (c), and the polynomial degree (n).

For each value of (k), the coefficients are obtained symbolically through determinant constructions involving evaluations of Meixner polynomials at

$$
-\beta,;
-\beta-1,;
\ldots,;
-\beta-k+1.
$$

---

## Contents

The repository contains implementations for

| Order | Computed coefficients |
| ----- | --------------------- |
| (k=1) | (A_1,B_1,D_1)         |
| (k=2) | (A_2,B_2,D_2)         |
| (k=3) | (A_3,B_3,D_3)         |
| (k=4) | (A_4,B_4,D_4)         |
| (k=5) | (A_5,B_5,D_5)         |
| (k=6) | (A_6,B_6,D_6)         |

Each section constructs:

1. the recurrence coefficients of Meixner polynomials;
2. the required evaluations of (M_n);
3. determinant cofactors;
4. the polynomial (G_2(x));
5. the coefficients (A_k), (B_k), and (D_k).

---

## Requirements

* Wolfram Mathematica 13.0 or later.

No external packages are required.

---

## Usage

Run the Mathematica script corresponding to the desired value of (k).

The program outputs

```Mathematica
Ak = ...
Bk = ...
Dk = ...
```

which are the exact symbolic expressions of the coefficients of

$$
G_2(x).
$$

---

## Output

For each modification order (k), the code returns the symbolic representation

$$
G_2(x)=A_kx^2+B_kx+D_k.
$$

The coefficients can subsequently be used for:

* discriminant analysis;
* zero localization;
* asymptotic investigations;
* numerical experiments;
* verification of theoretical results.

---

## Author

Eliya Ngabigala

Research interests:

* Orthogonal polynomials;
* Special functions;
* Spectral transformations;
* Meixner and discrete orthogonal systems.

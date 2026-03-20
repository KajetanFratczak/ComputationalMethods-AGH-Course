# 🧮 Computational Methods (MOwNiT) - AGH University

> Laboratory projects and assignments for the **Computational Methods in Science and Technology** (Metody Obliczeniowe w Nauce i Technice) course at AGH University.

This repository focuses on numerical analysis, algorithm optimization, floating-point arithmetic quirks, data visualization, and advanced numerical methods for solving mathematical problems. The main programming language used for computations is **Julia**, with data analysis and visualization handled in **R**.

## 👨‍💻 Author
* **Kajetan Frątczak**

---

## 🚀 Technologies & Tools
* **Julia** (DataFrames, Plots, Interpolations, Polynomials, LinearAlgebra, FFTW, DifferentialEquations)
* **R** (ggplot2)
* **Jupyter Notebook**

---

## 📁 Repository Contents

### 🔹 `lab1_2/` - Data Analysis & Benchmarking
* Introduction to `DataFrames` in Julia.
* Performance benchmarking of linear algebra operations (dot product, matrix-vector multiplication).

### 🔹 `lab3/` - Floating-Point Arithmetic
* Analysis of IEEE 754 floating-point representation (`Float16`, `Float32`, `Float64`).
* Investigating numerical instability and catastrophic cancellation.

### 🔹 `lab4/` - Data Visualization in R
* Data analysis and visualization using **R**.
* Generating performance plots with error bars (standard deviation) using `ggplot2`.

### 🔹 `lab5/` - Interpolation
* Implementation of polynomial interpolation methods: **Lagrange** and **Newton** (with Horner's scheme).
* Spline interpolation and demonstration of **Runge's phenomenon**.

### 🔹 `lab6/` - Approximation & Optimization
* Matrix multiplication optimization (comparing naive loops, loop interchange, and **BLAS**).
* Comparison of **Padé approximation** vs **Taylor series** for functions with singularities.

### 🔹 `lab7/` - Orthogonal Polynomials
* Generating and plotting **Hermite polynomials**.
* Analysis of basis functions and weight factors.

### 🔹 `lab8/` - Numerical Integration
* Implementation of **Legendre polynomials**.
* Exploring the connection between polynomial roots and **Gauss Quadrature** for numerical integration.

### 🔹 `lab9/` - Root Finding
* Solving non-linear equations using various methods: interval/sign change, derivative-based (Newton's method), and derivative approximations.
* Visualization of convergence and generation of **Newton's Fractal**.

### 🔹 `lab10/` - Linear Systems & QR
* Solving systems of linear equations comparing `inv()`, `\`, and `factorize()`.
* Implementation of the **QR factorization** algorithm and solving overdetermined systems.

### 🔹 `lab11/` - Iterative Solvers
* Implementation of iterative methods for solving linear systems: **Jacobi**, **Gauss-Seidel**, **SOR** (Successive Over-Relaxation), and **Chebyshev** iterations.
* Convergence and stability analysis.

### 🔹 `lab12/` - Ordinary Differential Equations (ODEs)
* Numerical solutions for ODEs using the **Euler method** and **Runge-Kutta** methods.
* Stability analysis for different time step sizes ($\Delta t$).
* Includes **visualizations and animations (.gif)** for dynamic systems like the Magnetic Pendulum, Predator-Prey models, and the SIR epidemiological model.

### 🔹 `lab13/` - Fast Fourier Transform (FFT)
* Signal processing and spectrum analysis (amplitude spectrum) using **FFT**.
* Noise removal and signal filtering using inverse FFT (`ifft`).
* Audio file processing (included `.wav` samples).

---

## ⚙️ How to run
The projects are provided as Jupyter Notebooks (`.ipynb`). To run the Julia notebooks, ensure you have the required packages installed in your Julia environment:
```julia
using Pkg
Pkg.add(["DataFrames", "Plots", "Interpolations", "Polynomials", "TaylorSeries", "FFTW", "DifferentialEquations"])
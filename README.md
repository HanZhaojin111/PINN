# PINN

This repository reproduces the PINN example for the nonlinear Schrödinger equation
(Section 3.1.1, continuous-time model).

## Setup

```bash
pip install -r requirements.txt
```

## Run the Schrödinger PINN example

```bash
python pinn_schrodinger.py --n0 50 --nb 50 --nf 20000 --lbfgs-max-iter 500 --save-predictions schrodinger_pinn.npz
```

The script trains a PINN with periodic boundary conditions and saves the predicted
solution on a regular grid (amplitude, real, and imaginary parts) into the `.npz`
file specified by `--save-predictions`.

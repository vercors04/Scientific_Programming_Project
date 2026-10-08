# Scientific_Programming_Project

Scientific programming project, M1 CSM course. Written in C, using the LAPACK library.

## Description

Solves the linear system Ax = b with LAPACKE (`LAPACKE_sgesv`, single precision), where A is the tridiagonal matrix with 2 on the diagonal and -1 on the off-diagonals, and every entry of b is h², with h = 1/(n+1).

For each n from 5 to 705 (step 50), the program writes the relative residual ‖Ax − b‖₁ / ‖b‖₁ and the execution time of the solve (in seconds).

## Files

| File | Content |
|---|---|
| `main.c`, `fct.c`, `header.h` | Main program, matrix functions, declarations |
| `code_mono.c` | Single-file version of the same program |
| `projet.sh` | Compiles `main.c` and `fct.c`, then runs the executable |
| `projetmono.sh` | Compiles `code_mono.c`, then runs the executable |
| `resultats n residu.txt` | n and relative residual |
| `resultats n tps execution.txt` | n and execution time (s) |
| `CR_PSC_KRSINAR_Xavier .pdf` | Report |
| `ennoncé.pdf` | Assignment statement |

## Build and run

Requires gcc and LAPACKE.

```bash
bash projet.sh
```

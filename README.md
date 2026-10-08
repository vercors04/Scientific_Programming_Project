# Projet_Programmation_Scientifique

Scientific programming project, M1 CSM course (Université de Rennes 1). Written in C, using the LAPACK library.

## Description

Solves dense linear systems AX = B with LAPACKE (`LAPACKE_sgesv`, single precision) for increasing matrix sizes n (5 to 705, step 50). For each n, the residual and the execution time are recorded.

## Files

| File | Content |
|---|---|
| `main.c`, `fct.c`, `header.h` | Main program, matrix functions, declarations |
| `code_mono.c` | Single-file version |
| `projet.sh` | Compiles and runs `main.c` and `fct.c` |
| `projetmono.sh` | Compiles and runs `code_mono.c` |
| `resultats n residu.txt` | Residual as a function of n |
| `resultats n tps execution.txt` | Execution time as a function of n |
| `CR_PSC_KRSINAR_Xavier .pdf` | Report |
| `ennoncé.pdf` | Assignment statement |

## Build and run

Requires gcc and LAPACKE.

```bash
bash projet.sh
```

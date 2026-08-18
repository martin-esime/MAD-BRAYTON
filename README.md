# Brayton el Loco - MAD-BRAYTON
### Calibrador Fortran 90 para condiciones iniciales GRMHD en régimen MAD

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21998449.svg)](https://doi.org/10.5281/zenodo.21998449)
**ESIME Azcapotzalco - IPN | Autor: Martín Hernández**

> Herramienta desarrollada en Fortran 90 que calibra perfiles de plasma en rotación alrededor de agujeros negros supermasivos. Validado con datos observacionales de M87* del Event Horizon Telescope.

### ¿Qué hace?
Evita simulaciones que nunca convergen a MAD. Usa el criterio de eficiencia de flujo magnético (phi_BH ~ 15) y el ciclo termodinámico Brayton como análogo energético.

### Validación
- Comparado con M87*: M = 6.5e9 M_sun, a* = 0.9, dotM = 2.7e-3 M_sun/yr
- Error < 5% vs modelos EHT GRMHD

### Citar
Si usas este código, por favor cita:
Hernández, M. (2026). MAD-BRAYTON v1.0. Zenodo. https://doi.org/10.5281/zenodo.21998449

### Instalación
```bash
gfortran -o mad_brayton mad_brayton.f90
./mad_brayton

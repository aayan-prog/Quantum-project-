# Quantum-project-
# ML-KEM AVX2 Optimized Engine

A high-speed, constant-time implementation of the ML-KEM (Kyber) polynomial arithmetic. 

## Features
- **Cooley-Tukey NTT** for forward transform.
- **Gentleman-Sande iNTT** for inverse transform (no bit-reversal needed).
- **AVX2 Vectorization** processing 16 coefficients per instruction.
- **Side-Channel Resistant**: No data-dependent branches or memory lookups.

## Performance (Intel Skylake+)
| Operation | Cycles |
|-----------|--------|
| NTT       | ~230   |
| iNTT      | ~215   |

## Usage
Include `poly.h` and compile with `-mavx2 -O3`.

# HEAANBOOT

- The code is implementation for Eurocrypt2018 paper.

- For current version of HEAAN please visit https://github.com/snucrypto/HEAAN

- You can also find this version in https://github.com/snucrypto/HEAAN/releases/tag/1.1

## PRNG Control

We add new encrypt method to select a seed:
```
Ciphertext Scheme::encryptMsg(Plaintext& msg, ZZ seed)
```

### Example

```
NTL::ZZ seed = ZZ(1);
Ciphertext cipher = scheme.encryptMsg(plain, seed);
```

## Dependencies

- GMP
  - On debian: sudo apt install libgmp10 libgmp-dev
- NTL
  - On debian: sudo apt install libntl-dev

## Instalation

cd HEAAN/lib
make -j$(nproc)

# License
Copyright (c) by CryptoLab inc. This program is licensed under a Creative Commons Attribution-NonCommercial 3.0 Unported License. You should have received a copy of the license along with this work. If not, see http://creativecommons.org/licenses/by-nc/3.0/.

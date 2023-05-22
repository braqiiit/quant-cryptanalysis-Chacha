# quant-cryptanalysis-Chacha

This repository consists of experiments on a Few Quantum Cryptanalysis Techniques.  
The folder structure is as follows:  
+ **ChaCha implementation**
  - `classical chacha.c`: Classical ChaCha cipher implementation in C  
  - `classical with addition.ipynb`: Notebook for classical ChaCha cipher implementation; easier to vary the number of bits in word size and constants  
  - `quantum rewired circuit.ipynb`: Our Final Quantum ChaCha implementation (uses Cuccaro et al.'04 for addition modulo 2^n, CNOT for XOR operations. rewiring for shift operations).
  - `qubit and gate count.ipynb`: Given a particular bit size, calculates the qubit count and depth of the circuit
+ **ChaCha cryptanalysis**
  - `ID OD bias.ipynb`: given a particular input difference and output difference position, generates the output difference
+ **Finding linear approximations**
  - `classicalSmallGIFT.c`: Generates the Linear approximation table for smallGIFT
  - `quant_SmallGIFT_LC.py`: Quantum implementation of smallGIFT cipher. Reference: https://github.com/tarunyadav/QuantumDifferentialAttack/blob/main/QuantumDifferentialCharacteristicsSearch.ipynb
  - `SmallGIFT linear crypt_shared.ipynb`: Finding linear approximations in smallGIFT cipher
  - `getting distribution.ipynb`: Generating the distribution of numbers for quantum smallGIFT 
  - `comparing classical and quantum histogram.ipynb`: To visualise the classical and quantum histograms of frequency of linear approximations

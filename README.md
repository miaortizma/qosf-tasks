# qosf-tasks
Pennylane implementation for task 1 and task 2 of QOSF task for batch 9 mentorship

Implementation for task 1 **(less than k)** is based on the following paper: [Automatic Generation of an Efficient Less-Than
Oracle for Quantum Amplitude Amplification, (Sanchez-Rivero et.al)](https://arxiv.org/pdf/2303.07120.pdf), which was fun to learn more in-depth about the Grover algorithm and the challenge of creating oracles. In my submission we explore the effect of the number of grover iterations, as well as set the stage with simpler single solution oracle

Task 2 **(odd-to-even)** was "easy" but I had a feeling of not being "quantum" enough as we just had to do an incomplete SWAP after the realization that you just need to turn the least significant qubit off, assuming X-gates encoding for each number. I based this only on knowledge of binary representation of numbers.

Based on the previous I decided to submit task 1 as my submission for QOSF mentorship, which seemed more completed.

Ideas for improvements to reduce circuit depth of MCZ can be based on: [Programmable networks for quantum algorithms
(Schuch&Siewert)](https://arxiv.org/abs/quant-ph/0303063) and the famous [Elementary gates for quantum computation (Barenco et.al)](https://arxiv.org/pdf/quant-ph/9503016.pdf)

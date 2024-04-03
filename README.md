# qosf-tasks
Pennylane implementation for task 1 of QOSF task for batch 9 mentorship

**Summary:**
Implementation for task 1 **(less than k)** is based on the following paper: [Automatic Generation of an Efficient Less-Than
Oracle for Quantum Amplitude Amplification, (Sanchez-Rivero et.al)](https://arxiv.org/pdf/2303.07120.pdf), which was fun to learn more in-depth about the Grover algorithm and the challenge of creating oracles. In my submission we explore the effect of the number of grover iterations, as well as set the stage with simpler single solution oracle. For this task we basically create a less-than-k oracle and find an appropiate number of iterations, which we ought to generalize as next steps).


**Next steps:**
Ideas for improvements to reduce circuit depth of MCZ can be based on: [Programmable networks for quantum algorithms
(Schuch&Siewert)](https://arxiv.org/abs/quant-ph/0303063) and the famous [Elementary gates for quantum computation (Barenco et.al)](https://arxiv.org/pdf/quant-ph/9503016.pdf). This is because the highest cost in our circuit comes from the MCX, which along with hadmard gates is used to create a multi-qubit controlled z operation, if we are able to reduce the depth from this MCX knowning that we want a MCZ, then we can greatly reduce circuit length

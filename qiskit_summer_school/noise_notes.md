video: understanding noise in near-term quantum computers

quantum computers suffer from hardware noise. it is important to understand where this noise comes from.

categories of noise:

- State preparation and measurement errors (SPAM)
  - this is an imperfect acquisition of the qubit state that can occur in **preparation** and **measurement**
- incoherent noise (2 types)
  - energy relaxation - the process of losing energy to the environment 1 -> 0 (T1)
  - dephasing - the process of superposition becoming classical. as the vector length gets smaller we lose information on the system. (T2)
  - pauli phase errors ???
- coherent noise
  - hamilton gate errors - misengineered hamiltonians can cause for incorrect gate rotations.
  - two-qubit gate errors - two-qubit compututions can sometimes have cross talk during computiations.

All of these errors make it highly important how circuits are designed to mitigage noise and understand the impact of noise on quantum hardware.

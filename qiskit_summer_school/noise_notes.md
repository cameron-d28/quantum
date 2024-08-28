steps of quantum computing:

- map classical inputs to quantum problem
- optimize quantum problem for execution
- execute on hardware with primitives (sampler or estimator)
- post-process results into classical

### video: understanding noise in near-term quantum computers

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

### video: limiting quantum noise

once better understanding where noise comes from, we can start to mitigate its effects.

approaches to limit noise:

- scientific approach
- engineering approach

ways to limit noise:

- make hardware better
- filter noisy results out

current practices for limiting noise:

- suppression (reduce the liklihood of errors and noise) [before computation]
  - dynamic decoupling (DD) ~ if qubits are idle put gates that cancel out crosstalk
  - Pauli Twirling (PT) ~ change noise to Pauli Channels that will in-turn stack up slower the original noise
- correction (fix and detect errors) [during computation]
- mitigation (filter out the noise after computation) [after computation]

noise can be mitigated in different steps of quantum computation (see above for details):

-

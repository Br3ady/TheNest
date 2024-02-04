# TheNest

This is our submission to the Quandela iQuHack 2024 In-Person Challenge. 

In our project, we built a somewhat functional QuGAN to help train an algorithms to produce a target state when given an input state. We used Quandela's solution for quantum computation with linear optics called Perseval to build out our solution. 

To do this, we first used Persval to build out the quantum circuit in [this paper](https://arxiv.org/abs/2310.00585) using Perseval's circuit tools. We reproduced the circuit from Figure 1.d of the Wang et al. paper using Perceval. Then, to construct the initial state, we used the Perseval class Statevector. In addition, we implemented the Fock space unitary by using a $$\frac{\ket{00} + \ket{11}}{\sqrt{2}}$$ input state to input into the Fock space unitary, before post-selecting for states where there was one photon in each ququart path. An attempt at using heralding was made using a series of Hadard and CNOT gates to replicate a CZ gate to generate the state $$\frac{\ket{00} + \ket{11}}{\sqrt{2}}$$ from a two photon input with two ancillary photons. 

After constructing the quantum circuit including the generator and discriminator, we used a GAN achine learning architecture to help train the generator and discriminator to compete against each other. 

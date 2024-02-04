# TheNest

This is our submission to the Quandela iQuHack 2024 In-Person Challenge. 

In our project, we built a somewhat functional QuGAN to help train an algorithms to produce a target state when given an input state. We used Quandela's solution for quantum computation with linear optics called Perseval to build out our solution. 

To do this, we first used Persval to build out the quantum circuit in [this paper](https://arxiv.org/abs/2310.00585) using Perseval's circuit tools. After constructing the quantu circuit including the generator and discriminator, we used a GAN achine learning architecture to help train the generator and discriminator to compete against each other. 

# Deep Reinforcement Learning

This repository is a simple example of:
 - deep-q-net (DQN)
 - asynchronous-advantage-actor-critic (A3C)
 
#### Simulation Environment

The simulator is a 4x4 square with 2 agents playing hide and seek.
The 1st agent needs to hide while the 2nd agent will try to chase.

Here is a random hide and seek example:

![random-example](asset/random.gif)

To change to a larger simulation grid,
one can simply change the `w` & `h` in `simulator.py`.
However, this will greatly affect the training time.

#### Strategy

The 1st agent is just a random decider in both examples.
The 2nd agent will be applied with DQN and A3C.

There are no significant improvement from DQN to A3C in this example.
Since there is no drastic state change in this simulation,
the value net will have little to help to stablize the advantage net.

I had also tried more complex network with Conv2D and MaxPool2D,
but it will take a lot longer for those structures to saturate.
Since we can get a viable result with a bare minimum Dense net,
we will take the training time save rather than accuracy in this DEMO.

#### Tech Stack

MxNet, Gluon
# minesweeper
# minesweeper

# dosp_2
# Project: Gossip and Push-Sum Algorithms with Actor-Based Simulation in Pony

## Team Members
- Chandan Abhishek Muchukota
- Vennela Priya Penumuchu
## What is Working
- **Gossip Algorithm**:
  - The rumor propagation algorithm works as expected, where actors select random neighbors to spread the rumor.
  - Termination criteria of receiving the rumor 10 times has been successfully implemented.
  - Gossip algorithm has been tested on all four topologies: Full Network, 3D Grid, Line, and Imperfect 3D Grid.
  
- **Push-Sum Algorithm**:
  - The sum computation through the Push-Sum algorithm has been implemented, where actors share their values (`s` and `w`) with random neighbors.
  - The ratio `s/w` converges within a precision of `10^-10` over three rounds.
  - The termination condition based on ratio convergence has been successfully tested on all topologies.
  
- **Topologies**:
  - We have successfully implemented the following topologies:
    1. **Full Network**: Each actor can communicate with every other actor.
    2. **3D Grid**: Actors are connected based on their position in a 3D grid.
    3. **Line**: Actors are connected sequentially in a linear fashion.
    4. **Imperfect 3D Grid**: Actors are in a 3D grid with one additional random connection per actor.
  
- **Performance Measurement**:
  - Convergence time is measured for both algorithms across different topologies using `System.currentTimeMillis()` to track the duration of execution.

## Largest Network Sizes Tested

For each algorithm and topology, the largest network size that the system could handle before performance degradation is noted below:

- **Gossip Algorithm**:
  - **Full Network**: Tested with up to **10,000 nodes**.
  - **3D Grid**: Tested with up to **10,000 nodes**.
  - **Line**: Tested with up to **10,000 nodes**.
  - **Imperfect 3D Grid**: Tested with up to **10,000 nodes**.

- **Push-Sum Algorithm**:
  - **Full Network**: Tested with up to **10,000 nodes**.
  - **3D Grid**: Tested with up to **10,000 nodes**.
  - **Line**: Tested with up to **10,000 nodes**.
  - **Imperfect 3D Grid**: Tested with up to **10,000 nodes**.

## Instructions for Running

To run the project, use the following command format:
```bash
./project2 <numNodes> <topology> <algorithm>

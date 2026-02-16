**Eyeriss Accelerator**  Eyeriss is a reconfigurable spatial architecture designed to accelerate Deep Convolutional Neural Networks (CNNs) by minimizing system-wide energy consumption, specifically targeting the high cost of data movement.

The core innovation is the **Row Stationary (RS)** dataflow, which maps computation to a 168-element  **PE** array in a way that maximizes local data reuse (**convolutional** , **filter**, and **Input feature map** (ifmap) reuse) within the PEs' local **Scratch Pads (Spads)**. By keeping filter rows and input feature map rows stationary inside the PEs, the architecture minimizes energy-expensive accesses to the on-chip **Global Buffer (GLB)** and off-chip DRAM.

The system features a specialized ***multicast*** **Network-on-Chip (NoC)** for efficient data distribution and employs **Run-Length Compression (RLC)** to exploit data sparsity (zeros) to further reduce DRAM bandwidth. 

Fabricated in 65nm CMOS, Eyeriss utilizes **Data Gating** to skip redundant zero-valued computations, achieving an energy efficiency of roughly 83 GMACS/W (at 1V) and significantly reducing the **DRAM access rate to 0.0029 accesses per MAC operation**.





**Hardware accelerator for AI** 
The paper's goal is to redesign MAC units ,as traditional mac units consumer lot of power .
Thus their Unit uses time domain signal processing instead of Analog or digital signal .

The chip is designed for **Inference** phase where The 'weights' are already known and loaded onto the chip to process new data . it does not deal with Training of the AI .

The authors argue that standard digital circuits have high capacitance​ because many bits toggle at once. Their Time-Domain approach compacts data into fewer wires, **reducing Capacitance** 

**TOPS/W (Tera-Operations Per Second per Watt):** The standard metric for energy efficiency in AI chips. Higher is better. This chip achieves **12.08 TOPS/W**

**Throughput (GOPS - Giga Operations Per Second):** How fast the chip processes data. This paper hits **0.365 GOPS** 

 The architecture features a **Bi-Directional Memory Delay Line (MDL)** that performs signed multiply-and-accumulate (MAC) operations by propagating pulses forward (for positive weights) or backward (for negative weights) through a chain of inverter-based delay units. Unlike prior analog approaches, this design is all-digital and capacitor-free, making it process-scalable and capable of near-threshold voltage operation (down to 375 mV). To address the inherent latency of time-domain processing, the authors introduce variable **Speed-up Modes** (1x–16x) that trade varying degrees of input quantization error for increased throughput. Additionally, the design includes a **Calibration Unit** to mitigate process-variation-induced delay mismatches and utilizes an Up/Down Counter as a Time-to-Digital Converter (TDC) to handle arithmetic overflows effectively. 
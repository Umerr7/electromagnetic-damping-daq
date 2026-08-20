# Data Acquisition System
<img width="3072" height="4080" alt="PXL_20260728_090040083(1)" src="https://github.com/user-attachments/assets/df5db7d0-14fa-415a-ba17-a47d2188022c" />
Measures mV level voltages and plots them on your computer screen, built using a raspberry pi pico and an OPA2134 op-amp signal conditioning stage, in order to plot accurate decay curves for an electromagnetic damping experiment with an active noise floor uncertainty of ±0.000034V. <br/><br/>

> see this project in action: [link]

I made this DAQ, because i was annoyed at the terrible analog oscilloscope in the lab where i was trying to conduct an electric damping experiment in which you pass a magnet through a coil to induce EMF. I did not realise how deeply this project would pull me in, and how how obsessed i would become at trying to condition the signal effectively. <br/>

# how to make your own!
<img width="3072" height="4080" alt="PXL_20260728_084321615" src="https://github.com/user-attachments/assets/df9b7698-cc3d-46fa-b593-478274b963c9" />

a "working" version of this device is quite simple, making a great version of this device is a lot harder. <br/>

feeding a constant voltage to the DAQ, and getting a quantized result with many "steps" of variation is inevitable when noise reduction measures have not been taken. <br/>

Most of the noise reduction is built in to the hardware and code. Keep all the wires short, the decoupling capacitors close to the pins, and ensure that the USB cable used to power the rasberry pi pico has its +5v bus cut off, and is instead powered through an external battery or power adapter. <br/>

<img width="566" height="835" alt="Screenshot from 2026-08-20 10-46-59" src="https://github.com/user-attachments/assets/75c1febf-af37-46eb-966a-4b9a36e2072a" />

[DAQ_electric_damp.pdf](https://github.com/user-attachments/files/31250556/DAQ_electric_damp.pdf)



# electric damping apparatus
<img width="3072" height="4080" alt="PXL_20260728_084732719" src="https://github.com/user-attachments/assets/5c4755c1-0d4d-458a-b15f-2ad6f0ce0077" />

A neodymium magnet is attached to a spring. An aluminum claw is used to release the magnet from a constant position with an initial velocity of zero. The magnet oscillates about the coil of wire, which induces EMF, Subsequently measured using the oscilloscope.  

# Stats
| Parameter | Specification |
| :--- | :--- |
| **ADC Bit Depth** | 12-bit (4,096 levels) |
| **Reference Voltage** | +3.3V DC |
| **Virtual Ground Bias** | +1.65V DC |
| **Hardware Step Resolution** | 0.806mV |
| **Input Voltage Ceiling** | ±47.14mV |
| **Hardware Gain** | 35x |
| **Active Noise Floor Uncertainty** |  ±0.034mV |
| **Signal-to-Noise Ratio (SNR)** | 58.9 dB |





# notes
A custom serial plotter was also made for this project by Hardyesh Kumar. It includes an extra post signal conditioning step called a **butterworth** filter

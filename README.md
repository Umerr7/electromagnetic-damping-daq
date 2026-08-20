# Data Acquisition System
<img width="3072" height="4080" alt="PXL_20260728_090040083(1)" src="https://github.com/user-attachments/assets/df5db7d0-14fa-415a-ba17-a47d2188022c" />
Measures mV level voltages and plots them on your computer screen, built using a raspberry pi pico and an OPA2134 op-amp signal conditioning stage, in order to plot accurate decay curves for an electromagnetic damping experiment with an active noise floor uncertainty of ±0.000034V.


|link to the video "see this project in action"

I made this DAQ, because i was annoyed at the terrible analog oscilloscope in my lab where i was trying to conduct an electric damping experiment in which you pass a magnet through a coil to induce EMF. I did not realise how deeply this project would pull me in, and how how obsessed i would become at trying to condition the signal effectively.

# how to make your own
<img width="3072" height="4080" alt="PXL_20260728_084321615" src="https://github.com/user-attachments/assets/df9b7698-cc3d-46fa-b593-478274b963c9" />

a "working" version of this device is quite simple, making a great version of this device is a lot harder. 

feeding a constant voltage to the DAQ, and getting a quantized result with many "steps" of variation is inevitable when noise reduction measures have not been taken.
Most of the noise reduction is built in to the hardware and code. Keep all the wires short, the decoupling capacitors close to the pins, and ensure that the USB cable used to power the rasberry pi pico has its +5v bus cut off, and is instead powered through an external battery or power adapter. 

[DAQ_electric_damp.pdf](https://github.com/user-attachments/files/31250556/DAQ_electric_damp.pdf)



# electric damping apparatus
[picture]
shortdescription

repeat for, springs - coils - magnet - claw

#specifications
specs

#notes
serial plotter, made by hardyesh
used a bit of AI

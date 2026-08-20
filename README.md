<img width="3072" height="4080" alt="PXL_20260728_090040083(1)" src="https://github.com/user-attachments/assets/df5db7d0-14fa-415a-ba17-a47d2188022c" />


# electromagnetic-damping-daq
A data acquisition (DAQ) system, optimized for electromagnetic damping, built using a raspberry pi pico and an opamp signal conditioning stage, in order to plot accurate decay curves with an active noise floor uncertainty of ±0.000034V.

In other terms: This is a custom-made digital oscilloscope, with a bunch of signal conditioning, to make it comparable to bench-top digital oscilloscopes for an electric damping experiment, where you pass a magnet through a coil to generate mV level EMFs, in order to observe EMF decay curves.

# how to make your own

a "working" version of this project is quite simple, making a great version of this project is a lot harder. 

feeding a constant voltage to the DAQ, and getting a quantized result with many "steps" of variation is inevitable when noise reduction measures have not been taken.

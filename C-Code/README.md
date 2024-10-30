# C-Code for inference

1.) Either run a new training with the Jupyter Notebook and generate a new MNIST model file 'trained_votes.h' or keep the existing file. 

2.) Draw a new MIST figure 'pixel_data.h' with 'pixel_painter.py' or keep the existing 'pixel_data.h'.

3.) Run 'make predict'. It should display a '6' as an inference result with the existing 'pixel_data.h'. Always compare 'pixel_data.h' "with your own eyes" (open it with an editor) with the inference result.

TODO: 
> Run this on microcontrollers - ESP32.
>
> Minimize 'trained_votes.h' in size.
>
> Run this in Verilog (Verilator) - codebase looks rather small, no bloated Python inference libraries (!).
>
> Dissect 'trained_votes.h' and make a qualified statement  about 'explainability' (ASCII file 1.6MB in size).

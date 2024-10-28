# Green Tsetlin Machine
Getting Sondre Glimsdal's Green Tsetlin Machine Framework to work "in under 10 minutes".

This project tries to simplify the assembly and evaluation process of a Green Tsetlin Machine that can train and classify images of the MNIST dataset. 

Sources:  
https://arxiv.org/abs/2405.04212  
https://green-tsetlin.readthedocs.io/en/latest/  
https://github.com/ooki/green_tsetlin

A Google Colab (Pro) notebook (.ipynb file) can be used to train and classify 28x28 pixel binary images.

A small Python script "Pixel Painter" can be used to draw the digits 0-9 and save the resulting 28x28 pixel image either as a .pkl or .h file.

A .h file (C-header) can be exported and used with a makefile to perform the inference using C-code only on a local computer.

To run the Google Colab (Pro) Python script: Upload the .ipynb file of this repo at Google Colab (Pro) and a pixel_data.pkl image file (a digit 0-9) you drew with Pixel Painter.

To run the inference with the C-backend: Download this repo and start the inference with "make predict" after you created a pixel_data.h file (a digit 0-9) with Pixel Painter.

TODO:  
> Colab Notebook + Pixel Painter  
    Makefile + .h + .c + Explanation, so it can be compiled with standard pixel_data.h  
    Documentation Colab Notebook - minus Hyperparameter sweep + Upload / Download  
    Size of .h file is result of number of clauses (!)
    ESP32 compatibility ?  
    FPGA Verilog / Verilator port with pixel painter add-on for Verilog array output  
    Export function for .h file is unique

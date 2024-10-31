# Green Tsetlin Machine
Getting Sondre Glimsdal's Green Tsetlin Machine Framework to work "in under 10 minutes".

This project tries to simplify the assembly and evaluation process of a Green Tsetlin Machine that can train and classify images of the MNIST dataset. 

Sources (Green Tsetlin Machine):  
https://arxiv.org/abs/2405.04212  
https://green-tsetlin.readthedocs.io/en/latest/  
https://github.com/ooki/green_tsetlin

Sources (MNIST dataset):  
https://botpenguin.com/glossary/mnist-dataset

With this project you have:

* A Google Colab (Pro) notebook (.ipynb file) that can be used to train and classify MNIST 28x28 pixel binary images.  

* A standalone C-program (.c file) that can be used to classify MNIST 28x28 pixel binary images.

* A small Python script (pixel_painter.py) that can be used to draw the digits 0-9 and save the resulting 28x28 pixel image either as a Python Pickle (.pkl) or C-header (.h) file.

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

# Green-Tsetlin-Machine
Getting Sondre Glimsdal's Green Tsetlin Machine Framework to work "in under 10 minutes"

Sources:  
https://arxiv.org/abs/2405.04212  
https://green-tsetlin.readthedocs.io/en/latest/  
https://github.com/ooki/green_tsetlin

This project tries to simplify the assembly and evaluation process of a Green Tsetlin Machine that can train and classify images of the MNIST dataset. 

A Google Colab (Pro) notebook (.ipynb file) can be used to train and classify 28x28 pixel binary images.

A small Python script "Pixel Painter" can be used to draw the digits 0-9 and save the resulting 28x28 pixel image either as a .pkl or .h file.

A .pkl (Pickle) file can be uploaded to the Google Colab (Pro) and classified by the notebook.

A .h file (C-header) can be exported and used with a makefile to perform the inference using C-code only on a local computer.

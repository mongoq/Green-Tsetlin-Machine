# Google Colab (Pro) Jupyter Notebook

With this notebook you can train the MNIST dataset for use with a Tsetlin machine.

After running a training you can either: 

*  Draw a digit with the Pixel Painter script, export it as 'pixel_data.pkl' image, upload it to Google Colab and run an inference there. This should yield a correct classification. 

Or: 

* Export the file 'trained_votes.h' (the MNIST model) to the 'C-Code' folder, add an image called 'pixel_painter.h' created with the Pixel Painter script, and run 'make predict'. This should yield a correct classification. 

# Hackaton2019

Team members: Harold Knoll, Rian Touchent, Armand Du Parc Locmaria, Kim NOEL

Last edit: March 31 2019

The files are:
* convert data minifold to python drawing.xls: This file is used to prepare the coordinates of the amine acid of the protein
* draw_protein_3.py: This file is used to draw in 3D the amine acid chain in 3D

## Context
The purpose is to plot in 3D the proteins avalaible in the project [MiniFold](https://github.com/EricAlcaide/MiniFold). The dataset was exctracted from [ProteinNet](https://github.com/aqlaboratory/proteinnet/blob/master/docs/proteinnet_records.md) project. 

In this projet we are able to plot the proteins in 3D based on the coordinates of the amine acids.


### Data on the proteins
The protein data are available [here](https://github.com/aqlaboratory/proteinnet) and the structure of the data is explained [here](https://github.com/aqlaboratory/proteinnet/blob/master/docs/proteinnet_records.md). The compressed folders can be extracted with 7-zip.

The data to retreive are located in the 'Tertiary structure section'. 


### convert data minifold to python drawing.xls
* Line 2 is to identify each 3x3 matrix
* From line 3 to 5 is to paste the text from the data of the Tertiary structure section
* Lines 7 to 10 are dedicated to replace the decimal separator, when needed
* Line 11 is used to paste the chain of amine acid. It is possible to split the string into multiple single symbol  by using the python function list(string)
* Lines 13 to 16 are used to concatenate the coordinates in a format easy to use in python script.
* Line 16 is used to concatenate the amine acids in a format easy to use in python script. 
* Cells B22 and B23 are to be copy and paste into the following python file into the variables *data* and *amine_acid*

### draw_protein_3.py
* Line 66 is where the processed data of the 3x3 matrices from the previous file can be paste
* Line 70 is where the processed data of the amine acid from the previous file can be paste


# QRcode-generator
Project Prerequisites
It is suggested that the developer has prior knowledge on Python and the Tkinter module. Also, use the below commands to install the qrcode and tkinter modules.

pip install tkinter
pip install qrcode
Steps to build the QR Code Generator in Python
To build the QR code generator project using Python we need to follow the below steps:
1. Importing the modules
2. Creating the main window
3. Taking the input of the text/URL, location to store the QR code, name of the QR code and the size of the QR code
4. Writing the function to generate and save the QR Code

1. Importing the modules
The first step is to import the qrcode and the tkinter module. We use the messagebox in the tkinter module to show the pop up messages.

import qrcode
from tkinter import *
from tkinter import messagebox
2. Creating the main window
Next, we create the main window with title, size and color.

#Creating the window
wn = Tk()
wn.title('DataFlair QR Code Generator')
wn.geometry('700x700')
wn.config(bg='SteelBlue3')
3. Taking the inputs
Now, we take the inputs from the user to create the QR Code. We take the following inputs:

1. Text/URL as Entry() named as ‘text’

2. Location to save the QR Code as Entry() named as ‘loc’

3. Name of the QR Code image when saved in the device as Entry() named as ‘name’

4. Size of the QR Code to be generated as Entry() named ‘size’. In this the user has to give the size in the range 1-40. 1 being the smallest size of 21×21.

Then we create a button when clicked generates the QR Code and saves it by executing the generateCode() function.


4. Creating the function to generate QR code and save it
Finally, we create the function to generate the code that runs on clicking the button. In this,

1. First we create the QRCode object with the version/size that user gave as input in the size() entry

2. Then we add the text that we need to encode by getting from the entry ‘text’

3. Then we get the QR code and save it in the directory that user gave as input

4. After this, we show the pop up message to confirm the user that the image is saved


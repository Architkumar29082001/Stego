# Stego
Overview
The provided Python code implements a simple Steganography (image-based) project using the Tkinter GUI library for the user interface and the Pillow (PIL) library for image processing. The application allows users to encode and decode hidden messages within images.

Classes
IMG_Stegno
This class represents the main functionality of the Steganography project.

Attributes
output_image_size An attribute to store the size of the input image during encoding.
Methods
main(self, root): Configures the main Tkinter window, sets up the UI components, and starts the Tkinter main loop.

back(self, frame): Destroys the current frame and returns to the main frame.

encode_frame1(self, F): Destroys the current frame and sets up the UI components for the first step of encoding.

decode_frame1(self, F): Destroys the current frame and sets up the UI components for the first step of decoding.

encode_frame2(self, e_F2): Takes an image file, displays it, and allows the user to enter a message for encoding.

decode_frame2(self, d_F2): Takes an image file, displays it, and decodes any hidden message.

decode(self, image): Decodes hidden data from an image using LSB (Least Significant Bit) method.

generate_Data(self, data): Converts characters of a message into binary format.

modify_Pix(self, pix, data): Modifies the pixel values of an image to hide data using LSB.

encode_enc(self, newImg, data): Encodes the provided data into the image.

enc_fun(self, text_a, myImg): Initiates the encoding process and saves the new image.

frame_3(self, frame): Destroys the current frame and returns to the main frame.

User Interface
The user interface is implemented using Tkinter, providing a simple layout with buttons and labels.
Buttons such as "Encode" and "Decode" trigger the corresponding actions.
Users can select image files for encoding or decoding using the "Select" button.
Text areas are provided for entering or displaying messages.


Dependencies
The code uses the Tkinter library for GUI, Pillow for image processing, and BytesIO for handling image data.


Usage
Run the script.
The main window appears with options to encode or decode.
Select "Encode" to hide a message in an image or "Decode" to reveal a hidden message.
Follow the on-screen instructions to select images and enter messages.
Save the output image with the hidden message.


Note
This documentation provides an overview of the code structure and functionality.
Ensure that the required libraries (Tkinter, Pillow) are installed before running the code.
The code may need adjustments based on future library updates or changes.
Customize and extend the code for additional features or improvements.

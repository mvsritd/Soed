# Soed
Steganograpphic Online Encoder/Decoder


the user chooses an image, the image data is then normalized, meaning that each RGB value is decremented by one if it is not even. This is done for every pixel in the image.

next the message is converted to a binary representation, 8 bits per character of the message. This binary representation is then applied to the normalized image, 3 Bit per pixel. This concludes, that the maximal length of a message hidden in an image is:

(Image Width * Image Height * 3)/8

Since the image was normalized, we now know that an even r, g or b value is 0 and an uneven is a 1. And this is how the message is decoded back from the image.

# Neural-style-transfer

## Goal:
Given an image, render it in the style of a given artist’s picture.



## Example:
Considered Katrina Kaif’s image as the content image to be rendered in the style of the art (1) Frida Kahlo, and (2) Mona Lisa.


## Core algorithm:
The loss function comprised of 3 main components:
- ‘content loss’: the L2 distance between representations of the given image and the resultant image,
- ‘style loss’: the sum of the L2 distances between the gram matrices of the 	representations of the style and resultant images from different layers of 	VGG16 network pretrained on ImageNet,
- ‘total variation loss’: imposes local spatial continuity between the pixels of 	the resultant image.

L-BFGS algorithm was used to minimize the loss.



## References:
Leon A. Gatys, Alexander S. Ecker, Matthias Bethge, “A Neural Algorithm of Artistic Style”.

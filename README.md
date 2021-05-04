# Document-Extraction : Shunya
1. Note the coordinates of the shape to be cropped by plotting the image using matplotlib
2. Build a polygon with the coordinates

# Addition
1. Mask the image, separating the largest contour with rest of the image
2. Make the background complete dark by applying bitwise_and on the cropped image with mask image as reference
3. Use bitwise not to transform this image with white background

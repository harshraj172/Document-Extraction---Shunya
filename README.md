# Document-Extraction : Shunya
1. Note the coordinates of the shape to be cropped by plotting the image using matplotlib
2. Build a polygon with the coordinates

# Addition
1. Mask the image, separating the largest contour with rest of the image
2. Apply bitwise_and on the cropped image with masked image as reference to make the background complete dark
3. Use bitwise_not to transform this image with white background

# Challenges
1. Due to the poor quality of images and a similar colored background around the object, automatic cropping failed to yield better results
2. The folded pages around the document failed the automatic scanning algorithm in detecting edges  

# Solution
1. We applied a semi automatic algorithm to detect the document 
2. Supervised learning with a relatively larger dataset containing documents in various orientation can produce a fully automated document scanner

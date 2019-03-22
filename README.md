# Document-Scanner
A Document scanner to scan the documents using mobile phone's camera utilising OpenCV , SKlearn, etc. libraries.
The whole procedure of this project can be divided into three steps:
1. Edge Detection:- Here, first we convert the image to grayscale, then blur it using gaussian_blur function, then the find out the edges using canny function. After this we get edged document.
2. Finding Contours:-  Find the contours in the edged image using the findContours function of opencv library, then keep only the largest ones, then find the contour having four points only i.e. rectangular in shape. Now, this is our Screen contour(outline) for the scanned image.
3. Apply a perspective transform and threshold:-  Apply the perspective transform on the outlined image using opencv library to get a rectangular top to bottom image. Finally apply threshold from sklearn library to get a decent black and white look of document.


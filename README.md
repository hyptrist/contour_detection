# box_contours_detection

 A contour line indicates a curved line representing the boundary of the same values or the same intensities. A contour map is the most straightforward example we can think of.

 Contour detection can be implemented by the functioncv2.findContours() in OpenCV and there are two important parameters here. mode is the way of finding contours, and method is the approximation method for the detection. 

 The mode cv2.RETR_TREE finds all the promising contour lines and reconstructs a full hierarchy of nested contours. The method cv2.CHAIN_APPROX_SIMPLE returns only the endpoints that are necessary for drawing the contour line. And as you can see above, this function gives the image, the detected contours and their hierarchy as its output.

 The returned contour is a list of points consisting of the contour lines. To draw the outer line of the figure, we’ll sort the contours by their area. With the selected contour line, cv2.drawContours() will depict the bounding line along with the points as shown below.

 There are more things we can do with the contour. We can find the centroid of an image or calculate the area of a boundary field with the help of the notion called image moment. What does a moment mean here? The word ‘moment’ is a short period of time in common usage. But in physics terminology, a moment is the product of the distance and another physical quantity meaning how a physical quantity is distributed or located. So in computer vision, Image moment is how image pixel intensities are distributed according to their location. It’s a weighted average of image pixel intensities and we can get the centroid or spatial information from the image moment.

 

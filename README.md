This javascript is developed to represent some contrast shapes on an image to a chain of points. Coordinates of this points can be used for drawing contour or filled shape on canvas. Algorithm require user to select a color of background and then automaticaly recognize an objects, outputing coordinates of it's contour points. 
Entire process consists of 4 stages:
1. Set transparent all pixels whitch colors are close enaugh to the defined bacgroubd color. Accurancy of this step is controlled by the tolerance value.
2. Go from initial point and find a first point of some object. The way of seaching is defined by spiral traectory.
3. Find a way along object boundary comparing color of object with transparet color of background.
4. Finaly contour consists of all pixels of object boundary. It's too much. An optimization remove unnecessary points and remain only ones lying on most curvature parts of contour.

You can test this code here; http://arybin.ru/autocontour

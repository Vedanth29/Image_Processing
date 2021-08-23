Connectivity-helps us to tell that which pixel are next to which. It helps to answer question like can we reach pixel 0 to pixel 1.
The concept of connectivity also helps simplify the definition of region or boundary in an image. 
Pixel connectivity describes a relation between two or more pixels.

----------------------------------------------------------------------------------------------------------------------------------

For two pixels to be connected they have to fulfill certain conditions on the pixel value and spatial adjacency.

*  The pixel brightness condition: Their pixel values must be from the same set of values C. For a grayscale image, C might be any range of possible gray-level values 0 to 255, e.g. C= {12,13,...40}, for a binary image we simply have C={1}.

 For a pixel p with the coordinates (x, y), the set of neighborhood pixels Nd (p) can be defined as follows:
 
 
 4- neighbors:

For a pixel p (x,y) shown in green circle, N4(p) is the set of 4-neigbors which share a face (or edge of the pixel) with p. They are four in number and are shown by orange circles. Two pixels p and q are 4-connected if q is in N4(p) and both p, q є C


8 –neighbors:

For a pixel p (x, y) shown in green circle, N8(p) is the set of neighbours which share a face or a vertex/corner. There are 8 such neighbours and they are shown by orange circles. Two pixels p and q are 8-connected if q is in N8(p) and both p,q є C


m –neighbors (mixed neighbors):

For a pixel p (x,y) shown in green circle, Nd(p) is the set of diagonal neigbors shown by red circles. Two pixels p and q with values from C are m-connected if:

q is in N4(p), or

q is in Nd(p), and the set N4(p) N4(q) has no pixels whose values are from C
---------------------------------------------------------------------------------------------------------------------------------------
Distance Metrics:

 On a discrete grid, the distance between two points a: (xa, ya) and b: (xb,yb) can be defined in a variety of ways.

*  Euclidean distance: In vector form, this is referred to as L2 norm.

*  City-block distance: This is the 4-connected distance and sometime called Manhattan distance.
   In vector form, it is referred to as L1 norm.

*  Chess-board distance: This is the 8-connected distance D8, also called as chess-board distance.






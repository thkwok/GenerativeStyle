To view the files, just drag and drop the *.field and *.design into the program.
Before that, the *.obj file should be imported (by drag and drop as well).

*.gradient is the gradient of streamline, which is defined by a series of vectors in the form of (x y z), ordered according to the face index.

*.field is the design field, which is defined by a series of field values, ordered according to the vertex index.

*.design is the styling file, which is defined by a set of curves, and each curve is defined by a set of edge nodes.
It starts with "curves #numCurve" to indicate how many curves in total.
It is followed by the first curve by "nodes #numNode" that indicates how many nodes in this curve.
Each edge node is defined as "#edgeid u", where #edgeid is the index of an edge, and "u" is the line parameter [0,1], i.e., (1-u)*s + u*e. "s" is the starting node, and "e" is the ending node of the edge.
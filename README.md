# New Strongly Regular Graphs

Edwin van Dam and Krystal Guo characterise strongly regular graphs of certain parameter classes, containing a "regular" point. This characterisation allows for the construction of many new strongly regular graphs. In particular, one can construct new strongly regular graphs of the following parameter classes:

(85,20,3,5) and (156,30,4,6).

As is explain in the paper, we could not do an exhausitive search of either class, but have come up with many examples. 

For the parameter class (85,20,3,5) we found 135478 graphs. The file newSRGs-85-20-3-5-w4.txt contains the graph6 strings of these graph, plus the point graph of W(4), which is the 76517th (indexing starts at 0). Each line is a graph6 string of a graph that has been canonically-labelled and the graphs have been ordered lexicographically by graph6 string. We note that two graphs are isomorphic if and only if the graph6 strings are equal, when they are both canonically labelled. 

For the parameter class (156,30,4,6) we found 17452 graphs. The file newSRGs-156-30-4-6-w5.txt contains the graph6 strings of these graph, plus the point graph of W(5), which is the 17452th (indexing starts at 0). Each line is a graph6 string of a graph that has been canonically-labelled and the graphs have been ordered lexicographically by graph6 string. 

# How to use these files 
 
Each line is a graph6 string of a graph that has been canonically-labelled. For example, in SageMath command line, one can do the following:

`sage: f = open("newSRGs-85-20-3-5-w4.txt","r")`

`sage: graphstrs = f.readlines()`

`sage: f.close()`

`sage: graphs = [Graph(j.strip("\n")) for j in graphstrs]`

`graphstrs` is a list of graph6 strings, which have the newline character "\n" at the end. Removing the extra characters, we will obtain a list, in this case `graphs`, of Graph objects in SageMath. 

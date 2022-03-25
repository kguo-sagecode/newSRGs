# New Strongly Regular Graphs

Edwin van Dam and Krystal Guo characterise strongly regular graphs of certain parameter classes, containing a "regular" point. This characterisation allows for the construction of many new strongly regular graphs. In particular, one can construct new strongly regular graphs of the following parameter classes:

(85,20,3,5) and (156,30,4,6).

As is explain in the paper, we could not do an exhausitive search of either class, but have come up with many examples. 

For the parameter class (85,20,3,5) we found 135478 new graphs. The files with `newSRGs-85-20-3-5` in the title contain the graph6 strings of these graphs. The graph6 string of the only previously known graph, which is the point graph of the generalized quadrangle W(4), in this class is given in `SRGs-85-20-3-5-w4.txt`. Each line is a graph6 string of a graph that has been canonically-labelled and the graphs have been ordered lexicographically by graph6 string. We note that two graphs are isomorphic if and only if the graph6 strings are equal, when they are both canonically labelled. 

For the parameter class (156,30,4,6) we found 27040 new graphs. The files with  `newSRGs-156-30-4-6` in the title contain the graph6 strings of these graphs. The graph6 string of the only previously known graph (with a regular point), which is the point graph of the generalized quadrangle W(5), in this class is given in `SRGs-156-30-4-6-w5.txt`.Each line is a graph6 string of a graph that has been canonically-labelled and the graphs have been ordered lexicographically by graph6 string. 

We also explicitly construct 1 new cospectral mate of GQ(q^2,q), which is give here for q=4,5; their parameters are:
(280,36,8,4) and (1105,80,15,5).

We also find a new cospectral mate for GQ(4,6). Again, classical GQ is given in SRG-125-28-3-7.txt and the new one is in newSRG-125-28-3-7.txt. 

# How to use these files 
 
Each line is a graph6 string of a graph that has been canonically-labelled. For example, in SageMath command line, one can do the following:

`sage: f = open("newSRGs-85-20-3-5-w4.txt","r")`

`sage: graphstrs = f.readlines()`

`sage: f.close()`

`sage: graphs = [Graph(j.strip("\n")) for j in graphstrs]`

`graphstrs` is a list of graph6 strings, which have the newline character "\n" at the end. Removing the extra characters, we will obtain a list, in this case `graphs`, of Graph objects in SageMath. 

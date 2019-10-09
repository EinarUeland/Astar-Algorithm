# Astar-Algorithm
An update of the Astar algorithm will be posted here

Can handle any heigth and width of occupancy grid? YES 
Possible to specify multiple goal nodes? YES. 
Fast and efficient? YES. 
Possible to specify connecting distance to other nodes? YES (in other words the algorithm is not restriced to 8-directions) 
There are no nested functions, subfunctions, plotters, or any other mess in the actual pathfinder script. 
Algorithm has simple inputs: An occupancy grid. A goal Matrix, the start node and preffered connecting distance. 


The provided code, allows for the user to set the connecting distance from each node themself. This means that the algorithm is not restriced to 4 or 8-directions (which often is the case in other implementations). In general a longer connecting distance require some more computation time.  

See the following examples for connecting distances varying between 1, 4 and 8;

<img src="https://github.com/EinarUeland/Astar-Algorithm/blob/TestRnd/Figures/ASTARSHOWCon1.png"   width="430" height="323"> <img src="https://github.com/EinarUeland/Astar-Algorithm/blob/TestRnd/Figures/ASt3arC1.gif"   width="430" height="323">

<img src="https://github.com/EinarUeland/Astar-Algorithm/blob/TestRnd/Figures/ASTARSHOWCon4.png"   width="430" height="323"> <img src="https://github.com/EinarUeland/Astar-Algorithm/blob/TestRnd/Figures/ASt3arC4.gif"   width="430" height="323">

<img src="https://github.com/EinarUeland/Astar-Algorithm/blob/TestRnd/Figures/ASTARSHOWCon8.png"   width="430" height="323"> <img src="https://github.com/EinarUeland/Astar-Algorithm/blob/TestRnd/Figures/ASt3arC10.gif"   width="430" height="323">


In this particular example, the A-Star algorithm needs to explore most cells. We can improve on efficiency by using the 2-sided solver as follows;  

<img src="https://github.com/EinarUeland/Astar-Algorithm/blob/TestRnd/Figures/2Sided.gif"   width="430" height="323"> 

Multiple goal nodes can be specified as the example above shows:

<img src="https://github.com/EinarUeland/Astar-Algorithm/blob/TestRnd/Figures/Multiple.gif"   width="430" height="323"> 

This could also be used for a "Frontier Based Exlporation" scheme in which the seacrch for the nearest. (note this is the case of the usage in the provided paper). 

<img src="https://github.com/EinarUeland/Astar-Algorithm/blob/TestRnd/Figures/FRONTIER.gif"   width="430" height="323"> 




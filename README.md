#This program is the implementation for A star algorithm 
The program reads in an input file, includes a optimal version and non-optimal version; This file will describe a set of cities, and your code will then allow the user to search for shortest paths between them using A∗ search. A city navigation file will have the following format:
name latitude longitude
<CITY NAME 1> <LAT 1> <LON 1>
  ...
<CITY NAME N> <LAT N><LON N>
 distances
<CITY NAME X1>, <CITY NAME Y1>: <MILES BETWEEN CITY X1 AND CITY Y1>
  ...
<CITY NAME XM>, <CITY NAME YM>: <MILES BETWEEN CITY XM AND CITY YM>

#What it does
This program will find the shortest path from start city S to goal city G, if such a path exists. When doing A∗ for any city C, the cost function g(C) is simply the total actual distance between start city S and C in the search so far. The heuristic value h(C) is given by the length of the shortest possible arc between C and goal G on the surface of the Earth. This is guaranteed to be an admissible and consistent heuristic for the data sets given, if calculated correctly. 

#Output
The program will output the total distance along that path (if no path exists this should be -1) And how many nodes it generated in the search (i.e., nodes ever placed into the frontier).How many nodes are left in the frontier (i.e. nodes that are never expanded)

 #Running
1. Compile all the classes
	  javac *.java

2. Run the optimized version or non optimized version
 	i.e   java OptSearch cities02.txt
	i.e   java NonOptSearch cities02.txt

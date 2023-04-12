# Introduction
* Please complete the following assessment using the R programming language (making use of any packages that you see fit)
    * Return your answer to your Full Fibre HR contact in a readable format that combines your code and output into one document (RMarkdown for example)
* **Please don't spend more than an hour on this technical assessment**
    * We would like to use it to help us assess how you approach and solve problems
    * Don't worry if you can't get to an answer - we are more interested in seeing what you tried and what your thought process was, so remember to comment your code!

## Data
* This repository contains two `.csv` files
    * `nodes.csv` the x and y coordinates of 6 points (nodes)
        * Variables
            * `id`: id of the node
            * `x`: x coordinate of the node
            * `y`: y coordinate of the node
            * `status`: status of the node
    * `edges.csv` the start and end points of 30 straight lines (edges)
    * These edges form a network
        * Variables
            * `id`: id of the line
            * `x_start`: the x coordinate of the start of the edge
            * `x_end`: the x coordinate of the end of the edge
            * `y_start`: the y coordinate of the start of the edge
            * `y_end`: the y coordinate of the end of the edge

# Question 1
* Read the `nodes.csv` and count the number of different `status` values there are
* Are any of the nodes missing a `status` value?

# Question 2
* Which of the nodes in `nodes.csv` are not within 150 m of any other node?
    * Assume all values are in metres

# Question 3 
* Compute the distance from each node to node 1 (`id = 1`) when travelling across the network edges provided in `edges.csv`
    * Assume there is no direction associated with the edges

# Question 4 
* If the nodes and edges provided in the .csv files were real points of interest for our fibre optic network in the UK, is there anything interesting you can say about them? 
    * Hint: We use the EPSG:27700 projected Coordinate Reference System (CRS): OSGB 1936 / British National Grid

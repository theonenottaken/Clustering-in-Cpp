# Clustering-in-Cpp

#### Summary of Project

The program divides a set of points in the two-dimensional plane into clusters by use of hierarchical clustering. In clustering algorithms, there are a number of ways
to calculate the distance between two clusters. This program supports two methods: single link and average link.

**Single link:** distance between two clusters is the shortest distance between a pair of elements from the two clusters.

**Average link:** distance between two clusters is the average distance between each pair of elements from the two clusters.

The program reads the input from a file in the current directory called “input.txt”. The first line of the file tells whether to use single link or average link, the
second line tells how many clusters to make, and all the subsequent lines are the set of points, with each point on a separate line. I have included four example input files
with the code. Note that the program always reads the file called “input.txt” so if you wish to change the input file, you must change the names of the files appropriately.
The program prints its output to a file called “output.txt”. The output is a list of numbers, each on a separate line, denoting which cluster the corresponding point from the
input file belongs to. For example, an output of...
1 2 2 1
 ...means that the point from the first line belongs to cluster 1, the point from the second line belongs to cluster 2, and so on.

#### How to Run

On a Linux system, download the files so that they’re all in one directory. Open a terminal and `cd`  to that directory. Type `make` and hit enter. Then type `./a.out` and hit enter.
That’s it! You should now find a new file in the directory called “output.txt”. The file contains the clusters that the points belong to, as described above.
You will also have a new executable file called “a.out” in the directory, along with many object files. If you wish to run the program again without recompiling, leave these files
in the directory and just enter `./a.out` again in the terminal. If you wish to get rid of these generated files, enter `make clean`. 

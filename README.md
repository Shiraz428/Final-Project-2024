# Final-Project-2024
CS_DataStructures_final_project
Shiraz and Hameed worked on this project

We used these sources for help:
https://www.youtube.com/watch?v=Glp7THUpGow and his source code: https://bitbucket.org/StableSort/play/src/master/src/com/stablesort/kdtree/KDTree.java
Wikipedia kdtree page - https://en.wikipedia.org/wiki/K-d_tree
javadoc
and ChatGpt

Report:

Word class:
  This class holds the word (String element) and a a float array called vec that stores the word vectors
  There is a getword method for returning the string

KDnode class:
  this is the node class for the kdtree
  It stores the word object, its left and right nodes and its depth (integer)
  It only has a constructor

kdnn class:
  This is the main class, we used the main method for testing
  This class contains the rootnode, depth and arraylist of word objects
  The buildfromfile method reads the textfile and constructs the kdtree from it, it reads each line and parses the word from its vectors
  The buildtree method is called by buildfromfile and sorts pairs of words based on the axis using compareTo method, it builds the tree recursively using the median word of the word list until words is empty
  The verifyAllWords method checks if all the words that were initially loaded from the input file are actually present in the k-d tree after it's been built, it checks if the size is the same as the number of words in the original input file and creates two hash sets to check if all of the words are the same in each
  The collect words method adds all of the words from a node and its subtrees to the words list
  The main method builds a kdtree and uses the verifyallwords method to check if the tree has been built correctly

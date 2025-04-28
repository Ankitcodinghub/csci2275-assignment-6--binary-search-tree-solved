# csci2275-assignment-6--binary-search-tree-solved
**TO GET THIS SOLUTION VISIT:** [CSCI2275 Assignment 6- Binary Search Tree Solved](https://www.ankitcodinghub.com/product/csci2275-csci-2270-ae-data-structures-assignment-6-binary-search-tree-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119710&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI2275 Assignment 6- Binary Search Tree Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Objectives

1. Build a binary search tree (BST)

2. Traversal, Search and Deletion in a BST

Instructions

Please read all the directions â€‹before writing code, as this write-up contains specific requirements for how the code should be written.

To receive credit for your code, you will need to pass the necessary test cases. Use the following steps to test your code as you work on the assignment:

1. Open up your Linux terminal, navigate to the build directory of this assignment (e.g. cd build).

2. Run the cmake .. command.

3. Run the make command.

4. If there are no compilation errors, two executables will be generated within the build directory: run_app_1 and run_tests.

5. If you would like to run your program, execute run_app_1 from the terminal by typing ./run_app_1 &lt;Required argument&gt;.

6. To run the grading tests, execute run_tests from the terminal by typing ./run_tests.

Overview

In 2009, Netflix held a competition to see who could best predict user ratings for films based on previous ratings without any other information about the users or films. The grand prize of US$1,000,000 was given to the BellKor’s Pragmatic Chaos team which bested Netflix’s own algorithm for predicting ratings by 10.06%. This kind of data science is facilitated with the application of good data structures. In fact, cleaning and arranging data in a conducive manner is half the battle in making successful predictions.

Imagine you are attempting to predict user ratings given a dataset of IMDBâ€™s top 100 movies. Building a binary search tree (BST) will enable you to search for movies and extract their features very efficiently. The movies will be accessed by their titles, but they will also store the following features:

IMDB ranking (1-100)

Title

Year released

IMDB average rating

Your binary search tree will utilize the following node struct:

struct MovieNode { int ranking; string title; int year; float rating; MovieNode* left = NULL; MovieNode* right

= NULL; };

MovieTree Class Specifications

Your code should implement a binary search tree (BST) of MovieNode data type. A header file that lays out this tree can be found in

NOTE: The test cases will be testing for memory leaks so take care of them to get full grades.

Fill in the file MovieTree.cpp according to the following specifications.

MovieTree() + Constructor: Sets root data member to NULL.

~MovieTree() + Destructor: Free all memory that was allocated and set root to NULL. void printMovieInventory() + Print every node in the tree in alphabetical order of titles using the following format:

cout &lt;&lt; “Movie: ” &lt;&lt; m-&gt;title &lt;&lt; ” (” &lt;&lt; m-&gt;rating &lt;&lt; “)” &lt;&lt; endl;

If there is no movie entry in the tree, print the following message instead:

cout &lt;&lt; “Tree is Empty. Cannot print.” &lt;&lt; endl;

void addMovieNode(int ranking, string title, int year, float rating) + Add a node to the BST in the correct place based on its title. Every nodeâ€™s left children should come before it alphabetically, and every nodeâ€™s right children should come after it alphabetically.

Hint: you can compare strings with &lt;, &gt;, ==, string::compare() function.

For example, if the root node of the tree is the movie â€œForrest Gumpâ€, then the movie â€œIron Manâ€ should be in the root’s right subtree and â€œAladdinâ€ should be in its left subtree.

You can assume that no two movies have the same title.

void findMovie(string title) + Find the movie with the given title, then print out its information:

cout &lt;&lt; “Movie Info:” &lt;&lt; endl; cout &lt;&lt; “==================” &lt;&lt; endl; cout &lt;&lt; “Ranking:” &lt;&lt; node-&gt;ranking &lt;&lt; endl; cout &lt;&lt; “Title :” &lt;&lt; node-&gt;title &lt;&lt; endl; cout &lt;&lt; “Year :” &lt;&lt; node-&gt;year &lt;&lt; endl; cout &lt;&lt; “Rating :” &lt;&lt; node-&gt;rating &lt;&lt; endl;

If the movie isnâ€™t found, print the following message instead:

cout &lt;&lt; “Movie not found.” &lt;&lt; endl;

void queryMovies(float rating, int year) + Print all the movies whose rating is at least as good as the input parameter rating and that are newer than year in the preorder fashion using the following format:

cout &lt;&lt; “Movies that came out after ” &lt;&lt; year &lt;&lt; ” with rating at least ” &lt;&lt; rating &lt;&lt; “:” &lt;&lt; endl; // each movie that satisfies the constraints should be printed with cout &lt;&lt; m-&gt;title &lt;&lt; ” (” &lt;&lt; m-&gt;year &lt;&lt; “) ” &lt;&lt; m&gt;rating &lt;&lt; endl;

If there is no movie entry in the tree, print the following message instead:

cout &lt;&lt; “Tree is Empty. Cannot query Movies.” &lt;&lt; endl; void averageRating() + Print the average rating for all movies in the tree. Use the following format:

cout &lt;&lt; “Average rating:” &lt;&lt; average &lt;&lt; endl;

If there is no movie entry in the tree, print the following message instead:

cout &lt;&lt; “Average rating:0.0” &lt;&lt; endl;

void printLevelNodes(int level) + Print all the nodes in the tree from left to right that are exactly at depth = level from the root of the tree. If the user passes a level value which is more than the maximum depth of the tree, then don’t print anything and just exit the function.

cout &lt;&lt; “Movie: ” &lt;&lt; m-&gt;title &lt;&lt; ” (” &lt;&lt; m-&gt;rating &lt;&lt; “)” &lt;&lt; endl;

For example, for the tree below, if level = 2, your function should print the title and rating for Akira, Batman and Hercules in that order (nodes from left to right at depth=2 from the root node of the tree).

Order of function implementation

1. Destructor and Constructor

2. addMovieNode and printMovieInventory

3. findMovie

4. queryMovies

5. averageRating

6. printLevelNodes

Main driver file [Main driver is provided in starter code]

NOTE: Main driver file is provided in starter code. You do not have to code it. We will walk through a brief introduction of the driver here

The main function will read information about each movie from a CSV file and store that information in a MovieTree using your addMovieNode() function implementation.

The name of the CSV file with this information should be passed in as a command-line argument. Example files Movies.csv, Documentaries.csv are added in the repository for your use in the format:

&lt;Movie 1 ranking&gt;,&lt;Movie 1 title&gt;,&lt;Movie 1 year&gt;,&lt;Movie 1 rating&gt; &lt;Movie 2 ranking&gt;,&lt;Movie 2 title&gt;,&lt;Movie 2 year&gt;,&lt;Movie 2 rating&gt; Etc…

After reading the information on each movie from the file and building the tree, the user is displayed the following menu:

======Main Menu====== 1. Find a movie 2. Query movies 3. Print the inventory 4. Average Rating of movies 5. Print movies at Level k 6. Quit

The menu options have the following behavior:

1. Find a movie: + Calls your treeâ€™s findMovie function on a movie specified by the user. The user is prompted for a movie title.

2. Query movies: + Calls your treeâ€™s queryMovies function on a rating and year specified by the user. Prompts the user for a rating and year.

3. Print the inventory: + Call your treeâ€™s printMovieInventory function

4. Average Rating of movies: + Calls your treeâ€™s averageRating function

5. Print movies at Level k: + Calls your treeâ€™s printLevelNodes function on the level specified by the user. The user is prompted for a level.

6. Quit: + Program exits after printing a friendly message to the user.
